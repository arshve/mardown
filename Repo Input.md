
# INPUT DROP DOWN
```JAVA
if (!CP_TYPE.equalsIgnoreCase("")) {
    Select inp_company_type = new Select(fluentWait(By.id("inp_company_type")));
    inp_company_type.selectByVisibleText(CP_TYPE);
    String value = inp_company_type.getFirstSelectedOption().getText();
    try {
        Assert.assertEquals(value, CP_TYPE);
        test.get().pass("<small>[Selectbox]</small> Company Type : " + value);
    } catch (AssertionError e) {
        test.get().fail("<small>[Selectbox]</small> Company Type : " + value);
        throw e;
    }
    Thread.sleep(500);
}
```

# INPUT TEXT 
```JAVA
if(!CP_NAME.equalsIgnoreCase("")) {
    WebElement x = fluentWait(By.id("inp_company_name"));
    x.sendKeys(Keys.HOME, Keys.chord(Keys.SHIFT, Keys.END), CP_NAME);
    String val = x.getAttribute("value");
    Assert.assertEquals(val, CP_NAME);
    test.get().pass("<small>[Textfield]</small> Company Name : " + val);
    Thread.sleep(500);
}
```


# INPUT KOTA AJAX
```JAVA
if(!CITY.equalsIgnoreCase("")) {
    WebElement inp_city_id = fluentWait(By.id("inp_city_id"));
    inp_city_id.clear();
    inp_city_id.sendKeys(CITY);
    String inp_city_idval = inp_city_id.getAttribute("value");
    try
    {
        Assert.assertEquals(inp_city_idval, CITY);
        test.get().pass("<small>[Input Textfield or Suggestion Tip]</small> City : " + inp_city_idval);
    }
    catch (AssertionError e)
    {
        test.get().fail("<small>[Input Textfield or Suggestion Tip]</small> City : " + inp_city_idval);
        throw e;
    }
    wait.until(ExpectedConditions.elementToBeClickable(By.xpath("//td[contains(., '" + CITY + "')]")));
    WebElement city = fluentWait(By.xpath("//td[contains(., '" + CITY + "')]"));
    city.click();
    Thread.sleep(500);
}
```

# INPUT MULTIPLE LANGUAGE FIELD
```JAVA
if (!NAME.equalsIgnoreCase("")) {
    String[] st_desc = NAME.split(", ");
    String[] lang = LANG.split(", ");
    for(int i = 0;i < st_desc.length;i++)
    {
        WebElement x = fluentWait(By.id("inp_pos_name_" + lang[i]));
        x.sendKeys(Keys.HOME, Keys.chord(Keys.SHIFT, Keys.END), st_desc[i]);
        Thread.sleep(500);
        String val = x.getAttribute("value");
        Assert.assertEquals(val, st_desc[i]);
        test.get().pass("<small>[Input Textfield]</small> Unit Name : " + st_desc[i]);
    }
    Thread.sleep(1000);
}
```
# INPUT ATTACHMENT
```JAVA
if(!ATTACHMENT.equalsIgnoreCase("")) {
    WebElement inp_filename_new = fluentWait(By.id("inp_filename_new"));
    inp_filename_new.sendKeys(curr + ATTACHMENT);
    Thread.sleep(500);
    String[][] data = {
            {"<small>[Attach]</small>"},
            {"<b>File Attachment</b>"},
            {ATTACHMENT}
    };
    test.get().pass(MarkupHelper.createTable(data));
}
```

#   Select Radio Button
```JAVA
WebElement inp_pos_flag = fluentWait(By.xpath("//input[@name='inp_pos_flag' and @title='Job Position']"));
inp_pos_flag.click();

String inp_pos_flagval = inp_pos_flag.getAttribute("title");
try {
    Assert.assertEquals(inp_pos_flagval, "Job Position");
    String[][] data = {
            {"<small>[Radio Button]</small>"},
            {"<b>Position Flag</b>"},
            {inp_pos_flagval}
    };
    test.get().pass(MarkupHelper.createTable(data));
} catch (AssertionError e) {
    test.get().fail(MarkupHelper
            .createCodeBlock("Position Flag \n[EXPECTED] : Job Position, [ACTUAL] : " + inp_pos_flagval));
    throw e;
}
Thread.sleep(500);
```

#   Check Box
```JAVA
WebElement check = driver.findElement(By.id("inp_pos_active"));
for(int i=0; i<2; i++) {
    check.click();
    test.get().pass("<small>[Textfield]</small> Check Box Clicked");
}
```
```JAVA
if (!STATUS.equalsIgnoreCase("Active")) {
    WebElement inp_pos_active = fluentWait(By.id("inp_pos_active"));
    inp_pos_active.click();
    Thread.sleep(500);
    if (!inp_pos_active.isSelected()) {
        test.get()
                .pass(MarkupHelper.createCodeBlock("[Checkbox] Active : Unchecked"));
    } else {
        test.get().fail(MarkupHelper.createCodeBlock("Failed Unchecked [Checkbox] Active"));
    }
}
```

# Insert Multiple input To Right Box
```JAVA
if (!GRADE.equalsIgnoreCase("")) {
    String[] typeofL = GRADE.split(", ");
    for (String eltypeofL : typeofL) {
        if (eltypeofL != null && eltypeofL.length() > 0) {
            WebElement tol = fluentWait(By.id("inp_lstgradecode"));
            tol.sendKeys("");
            tol.sendKeys(eltypeofL);
            Thread.sleep(8000);
            WebElement found = fluentWait(By.cssSelector("#unselinp_lstgradecode > option:nth-child(1)"));
            actions.doubleClick(found).perform();
            Thread.sleep(3000);
            tol.clear();
            Thread.sleep(500);
            String[][] data = {
                    {"<small>[Multiple Selectbox]</small>"},
                    {"<b>Grade</b>"},
                    {eltypeofL}
            };
            test.get().pass(MarkupHelper.createTable(data));
        }
    }
}
```

# Conditional Radio Button
```JAVA
if (OPT_TO_REJECT.equalsIgnoreCase("Yes")) {
    WebElement inp_pos_flag = fluentWait(By.xpath("//input[@id='inp_give_option_reject' and @title='Yes']"));
    inp_pos_flag.click();
    String inp_pos_flagval = inp_pos_flag.getAttribute("title");
    try {
        Assert.assertEquals(inp_pos_flagval, "Yes");
        String[][] data = {
                {"<small>[Radio Button]</small>"},
                {"<b>Position Flag</b>"},
                {inp_pos_flagval}
        };
        test.get().pass(MarkupHelper.createTable(data));
    } catch (AssertionError e) {
        test.get().fail(MarkupHelper
                .createCodeBlock("Position Flag \n[EXPECTED] : Yes, [ACTUAL] : " + inp_pos_flagval));
        throw e;
    }
} else {
    WebElement inp_pos_flag = fluentWait(By.xpath("//input[@id='inp_trackable_acceptance' and @title='No']"));
    inp_pos_flag.click();
    String inp_pos_flagval = inp_pos_flag.getAttribute("title");
    try {
        Assert.assertEquals(inp_pos_flagval, "Track Acceptance");
        String[][] data = {
                {"<small>[Radio Button]</small>"},
                {"<b>Position Flag</b>"},
                {inp_pos_flagval}
        };
        test.get().pass(MarkupHelper.createTable(data));
    } catch (AssertionError e) {
        test.get().fail(MarkupHelper
                .createCodeBlock("Position Flag \n[EXPECTED] : No, [ACTUAL] : " + inp_pos_flagval));
        throw e;
    }
}
```
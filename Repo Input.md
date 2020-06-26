Menu +[TASK](https://github.com/arshve/mardown/blob/master/Task.md)+ +[Repo Input](https://github.com/arshve/mardown/blob/master/Repo%20Input.md#Insert-Multiple-input-To-Right-Box)+ +[Repo Button](https://github.com/arshve/mardown/blob/master/Repo%20Button.md)+ +[Repo Documentation](https://github.com/arshve/mardown/blob/master/Repo%20Documentation.md)+ +[Repo Select By](https://github.com/arshve/mardown/blob/master/Repo%20Select%20By.md)+ +[Repo Select](https://github.com/arshve/mardown/blob/master/Repo%20Select.md)+ +[ModulSF List](https://github.com/arshve/mardown/blob/master/ModulSF6.md)+

# SP6 ERP Selenium **Input** Repo

1. [Input Drop Down](#Input-Drop-Down)
2. [Input Text](#Input-Text)
3. [Input Kota Ajax](#Input-Kota-Ajax)
4. [Input Multiple Language](#Input-Multiple-Language)
5. [Attachment](#Input-Attachment)
6. [Check Box](#Check-Box)
7. [Insert Multiple Select input To Right Box](#Insert-Multiple-input-To-Right-Box)

---

## Input Drop Down

<details>
<summary> Code! </summary>

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

<details>
<summary> What is Look Like! </summary>

![Example](https://i.ibb.co/bmMNvTT/Drop-Down-Input.png)

</details>

</details>

## Input Text

<details>
<summary> Code! </summary>

```JAVA
if(!CP_NAME.equalsIgnoreCase("")) {
   WebElement element = (new WebDriverWait(driver, 10))
    .until(ExpectedConditions.elementToBeClickable(By.id("inp_cat_code")));
    element.clear();
    Thread.sleep(500);
    element.sendKeys(Keys.HOME, Keys.chord(Keys.SHIFT, Keys.END), CP_NAME);
    String val = element.getAttribute("value");
    Assert.assertEquals(val, CP_NAME);
    test.get().pass("<small>[Textfield]</small> Company Name : " + val);
    Thread.sleep(500);
}
```

#### With Ajax

```JAVA
if (!PARENT.equalsIgnoreCase("")) {
   WebElement element = (new WebDriverWait(driver, 10))
    .until(ExpectedConditions.elementToBeClickable(By.id("inp_cat_code")));
    element.clear();
    Thread.sleep(500);
    element.sendKeys(PARENT);
    Thread.sleep(2000);
    fluentWait(By.xpath("//td[contains(., '" + PARENT + "')]")).click();
    Thread.sleep(1500);
    test.get().pass("Parent Code : " + PARENT);
    Thread.sleep(1500);
}
```

<details>
<summary> What is Look Like! </summary>

![Example](https://i.ibb.co/0DK0KLB/Text-Input.png)

</details>

</details>

## Input Kota Ajax

<details>
<summary> Code! </summary>

```JAVA
if(!CITY.equalsIgnoreCase("")) {
    WebElement element = (new WebDriverWait(driver, 10))
    .until(ExpectedConditions.elementToBeClickable(By.id("inp_cat_code")));
    element.clear();
    Thread.sleep(500);
    element.sendKeys(CITY);
    String inp_city_idval = element.getAttribute("value");
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
    Thread.sleep(1500);
    city.click();
}
```

<details>
<summary> What is Look Like! </summary>

![Example](https://i.ibb.co/qdRNmP9/City-Ajax-Input.png)

</details>

</details>

## Input Multiple Language

<details>
<summary> Code! </summary>

```JAVA
if (!NAME.equalsIgnoreCase("") && jr2 == true) {
    String[] st_desc = NAME.split(", ");
    String[] lang = LANG.split(", ");
    for(int i = 0;i < st_desc.length;i++)
    {
        WebElement element = (new WebDriverWait(driver, 10))
        .until(ExpectedConditions.elementToBeClickable(By.id("feedback_name_"+ lang[i] +"_"+ xpathCount)));
        element.clear();
        Thread.sleep(500);
        element.sendKeys(Keys.HOME, Keys.chord(Keys.SHIFT, Keys.END), st_desc[i]);
        Thread.sleep(500);
        String val = element.getAttribute("value");
        Assert.assertEquals(val, st_desc[i]);
        test.get().pass("<small>[Input Textfield]</small> Feedback Name ["+lang[i]+"]: " + st_desc[i]);
    }
    Thread.sleep(1000);
}
```

### Multiple Language Field With FCK Text Editor

```JAVA
if (!VISION.equalsIgnoreCase("")) {
    String[] st_desc = VISION.split(", ");
    String[] lang = LANG.split(", ");
    for(int i = 0;i < st_desc.length;i++) {
        try {
            wait.until(ExpectedConditions.frameToBeAvailableAndSwitchToIt(By.xpath("//*[@id=\"inp_vision_"+ lang[i] +"___Frame\"]")));
            wait.until(ExpectedConditions.frameToBeAvailableAndSwitchToIt(By.xpath("//*[@id=\"xEditingArea\"]/iframe")));
            WebElement body = driver.findElement(By.tagName("body"));
            if(body != null) {
                System.out.println("body "+i+" exist");
            } else {
                System.out.println("body "+i+" not exist");
            }
            System.out.println(lang[i]); // debug
            System.out.println(st_desc[i]); // debug
            body.clear();
            body.sendKeys(st_desc[i]);
            Thread.sleep(500);
            test.get().pass("<small>[Input FCK Text Editor]</small> Vision : " + st_desc[i]);
            driver.switchTo().parentFrame();
        } catch(Exception e) {
            System.out.println("Error. "+e.getMessage());
        }
        System.out.println("loop "+i); // debug
        driver.switchTo().parentFrame();
    }
    Thread.sleep(500);
}
```

<details>
<summary> What is Look Like! </summary>

#### Standard

![Example](https://i.ibb.co/qNVJ5XK/Standard-Language-Input.png)

#### FCKEditor

![Example](https://i.ibb.co/HGmSDQ6/FCKEditor-Input.png)

</details>

</details>

## Input Attachment

<details>
<summary> Code! </summary>

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

<details>
<summary> What is Look Like! </summary>

![Example](https://i.ibb.co/WgF2C8n/Attachment.png)

</details>

</details>

## Select Radio Button

<details>
<summary> Code! </summary>

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

### Conditional Radio Button

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

<details>
<summary> What is Look Like! </summary>

![Example](https://i.ibb.co/H27CdgT/Radio-Box-Input.png)

</details>

</details>

## Check Box

<details>
<summary> Code! </summary>

### Double Click Check

```JAVA
WebElement check = driver.findElement(By.id("inp_pos_active"));
for(int i=0; i<2; i++) {
    check.click();
    test.get().pass("<small>[Textfield]</small> Check Box Clicked");
}
```

### Single Click Check

```JAVA
if (REQ.equalsIgnoreCase("Active")) {
    WebElement inp_pos_active = fluentWait(By.id("inp_is_newhire"));
    inp_pos_active.click();
    Thread.sleep(500);
    if (!inp_pos_active.isSelected()) {
        test.get().pass(MarkupHelper.createCodeBlock("[Checkbox] Active : Unchecked"));
        inp_pos_active.click();
    } else {
        test.get().fail(MarkupHelper.createCodeBlock("Failed Unchecked [Checkbox] Active"));
    }
}
```

<details>
<summary> What is Look Like! </summary>

![Example](https://i.ibb.co/Yy1Vqhr/Check-Box-Input.png)

</details>

</details>

## Insert Multiple input To Right Box

<details>
<summary> Code! </summary>

### With Search

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

### Without Search

```JAVA
if (!ORG_UNIT.equalsIgnoreCase("")) {
        String[] split = ORG_UNIT.split(", ");
        for(int i = 0;i < split.length;i++){
            Select item = new Select(driver.findElement(By.xpath("//*[@id=\"unselinp_division\"]")));
            item.selectByVisibleText(split[i]);
            Thread.sleep(300);
            test.get().pass("Provider " +split[i]+" Added");
        }
        WebElement found = fluentWait(By.cssSelector("#tr_inp_grade > td:nth-child(2) > table:nth-child(4) > tbody:nth-child(1) > tr:nth-child(1) > td:nth-child(2) > input:nth-child(1)"));
        found.click();
}
Thread.sleep(1000);
```

### Without Search + Validation Data

<details>
<summary> Initiate! </summary>

```JAVA
public boolean isElementPresent(By by) {
    try {
    driver.findElement(by);
    return true;
    } catch (NoSuchElementException e) {
    return false;
    }
}
```

</details>

```JAVA
if (!GRADE_LIST.equalsIgnoreCase("")) {
    String[] split = GRADE_LIST.split(", ");
    for(int i = 0;i < split.length;i++){
        boolean exists = driver.findElements(By.xpath("//option[@title='" + split[i] + "']")).size() != 0;
        if (exists) {
            Select item = new Select(driver.findElement(By.id("unselinp_acsmember")));
            item.selectByVisibleText(split[i]);
            test.get().pass("<small>[Grade List]</small> "+ split[i] +" Added");
            Thread.sleep(300);
        } else {
            System.out.println(split[i] +" Doesnt Found");
            test.get().pass("<small>[Grade List]</small> "+ split[i] +" Not Found");

        }
    }
    WebElement found = fluentWait(By.cssSelector("html body#pageBodyHRM.fullsize div#divBlock.divBlock div#divPopup.divPopup table#formtable tbody tr td"
            + "#pop_data.box div#formspace div form#frmGradeCategory div#divForm fieldset table tbody tr#tr_inp_acsmember.clTR1 td#tdb_1 table tbody tr td input"));
    found.click();

}

```

#### Referse Without Search

```JAVA
boolean jobFam = isElementPresent(By.cssSelector("#selinp_acsmember > option:nth-child(1)"));
System.out.println(jobFam);

if(jobFam) {
    Select select = new Select(driver.findElement(By.id("selinp_acsmember")));
    List <WebElement> elementCount = select.getOptions();
    int iSize = elementCount.size();
    for(int i =0; i<iSize ; i++){
        String sValue = elementCount.get(i).getText();
        System.out.println(sValue);
        select.selectByVisibleText(sValue);
        Thread.sleep(300);
    }
    WebElement found = fluentWait(By.cssSelector("#tr_inp_acsmember > td:nth-child(2) > table:nth-child(4) > tbody:nth-child(1) > tr:nth-child(1) > td:nth-child(2) > input:nth-child(4)"));
    found.click();
    System.out.println(jobFam);
}
test.get().pass("Undo the Title Grade");
Thread.sleep(500);
```

Initiate Condition

```JAVA
public boolean isElementPresent(By by) {
    try {
        driver.findElement(by);
        return true;
    } catch (NoSuchElementException e) {
        return false;
    }
}
```

<details>
<summary> What is Look Like! </summary>

#### With Search Box

![Example](https://i.ibb.co/554tVtV/Multiple-Select-with-search.png)

#### Without Search Box

![Example](https://i.ibb.co/NL9PBqS/Multiple-Select-Without-search.png)

</details>

</details>

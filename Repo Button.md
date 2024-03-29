Menu +[TASK](https://github.com/arshve/mardown/blob/master/Task.md)+ +[Repo Input](https://github.com/arshve/mardown/blob/master/Repo%20Input.md#Insert-Multiple-input-To-Right-Box)+ +[Repo Button](https://github.com/arshve/mardown/blob/master/Repo%20Button.md)+ +[Repo Documentation](https://github.com/arshve/mardown/blob/master/Repo%20Documentation.md)+ +[Repo Select By](https://github.com/arshve/mardown/blob/master/Repo%20Select%20By.md)+ +[Repo Select](https://github.com/arshve/mardown/blob/master/Repo%20Select.md)+ +[ModulSF List](https://github.com/arshve/mardown/blob/master/ModulSF6.md)+

## Submit Button

## With Alert Check

```JAVA
Thread.sleep(500); // TimeOut
takeScreenShot(TC_ID, SC_TYPE, TC_ID);
test.get().addScreenCaptureFromPath(filePathSc + TC_ID + ".png");
Thread.sleep(500); // TimeOut
fluentWait(By.id("btn_a_2")).submit();
Thread.sleep(3000); // TimeOut
test.get().pass("<small>[button]</small> Submit clicked, then Alert Appeared");
WebDriverWait wait_alert = new WebDriverWait(driver, 10 /* timeout in seconds */);
if (wait_alert.until(ExpectedConditions.alertIsPresent()) == null) {
    System.out.println("alert was not present!");
    test.get().fail("Alert was not present!");
} else {
    Alert alert = driver.switchTo().alert();
    test.get().pass(MarkupHelper.createLabel("Accept Alert Evidence : " + alert.getText(), ExtentColor.ORANGE));
    String alertval = alert.getText();
    if(alertval.contains("Successfully") && TEST_CASE_TYPE.equalsIgnoreCase("P")) {
        alert.accept();
        Thread.sleep(3000); // TimeOut
    } else if(!alertval.contains("Successfully") && TEST_CASE_TYPE.equalsIgnoreCase("N")) {
        alert.accept();
        driver.switchTo().defaultContent();
        Thread.sleep(3000); // TimeOut
        driver.navigate().refresh();
        Thread.sleep(3000); // TimeOut
    } else {
        alert.accept();
        driver.navigate().refresh();
        Thread.sleep(3000); // TimeOut
        Assert.fail("Unexpected Alert Appeared. Test Case Type is "+ TEST_CASE_TYPE + " , but alert text is " + alertval);
    }
    Thread.sleep(4000); // TimeOut
}
```

---

## Without Alert Check

```JAVA
WebElement submit = fluentWait(By.id("btn_a_2"));
submit.click();
test.get().pass("<small>[Button]</small> Mengklik Submit");
Thread.sleep(4000); // TimeOut
//handle alert
takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_1"); // Report
test.get().pass("Submited", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_1.png").build());
resolveAllAlerts(driver, 16, true);
Thread.sleep(4000); // TimeOut
```

---

## Delete Button

```JAVA
driver.switchTo().parentFrame();
WebElement submit = fluentWait(By.id("btn_a_1"));
submit.click();
Thread.sleep(4000); // TimeOut
test.get().pass("<small>[Button]</small> Mengklik Delete");
//handle alert
resolveAllAlerts(driver, 16, true);
Thread.sleep(4000); // TimeOut
```

# ScreenShoot & Close Second Window

> [Source](https://stackoverflow.com/questions/9588827/how-to-switch-to-the-new-browser-window-which-opens-after-click-on-the-button)

```JAVA
// Store the current window handle
String winHandleBefore = driver.getWindowHandle();

// Perform the click operation that opens new window
WebElement log = fluentWait(By.id("btn_a_1"));
log.click();
Thread.sleep(4000); // TimeOut
// Switch to new window opened
for(String winHandle : driver.getWindowHandles()){
    driver.switchTo().window(winHandle);
}

// Perform the actions on new window
takeScreenShot(TC_ID, SC_TYPE, TC_ID + "[Unik Id]"); // Report
test.get().pass("[Message]", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "[Unik Id].png").build());

// Close the new window, if that window no more required
driver.close();
Thread.sleep(3000); // TimeOut
// Switch back to original browser (first window)
driver.switchTo().window(winHandleBefore);
```

# Click Code with LineText

```JAVA
try {
    WebElement code = driver.findElement(By.linkText("TestGradeCat"));
    code.click();
}
catch(org.openqa.selenium.StaleElementReferenceException ex)
{
    WebElement code = driver.findElement(By.linkText("TestGradeCat"));
    code.click();
}
```

# ROBOT Press Enter

> [Source](https://stackoverflow.com/questions/23734691/how-to-press-enter-without-targeting-a-webelement)

```JAVA
try {
    Robot robot = new Robot();
    robot.keyPress(KeyEvent.VK_ENTER);
    robot.keyRelease(KeyEvent.VK_ENTER);
    robot.delay(200);
}

// Or

Actions builder = new Actions(driver);
builder.keyDown(Keys.RETURN).keyUp(Keys.RETURN).build().perform();

```

# Alert Handling

```JAVA

//			Handling Alert
try {
    wait.until(ExpectedConditions.alertIsPresent());
    Alert alert = driver.switchTo().alert();
    // get the message which is present on pop-up
    String message = alert.getText();
    // print the pop-up message
    test.get().pass(MarkupHelper.createCodeBlock("[Alert] "+message));
    System.out.println(message);
    // Accept Alert
    alert.accept();
} catch (Exception e) {
    //exception handling
    test.get().fail(MarkupHelper.createCodeBlock("Alert Not Showing Up :" +e));
}
Thread.sleep(4000);

```

# Checkbox Verification

```JAVA

private boolean isChecked;

isChecked = driver.findElement(By.id("iscat_"+st_desc[i])).isSelected();
if(isChecked) {
    test.get().pass("<small>[Checkbox]</small> row "+st_desc[i]+" Already Category");
}else {
    WebElement cateAdd = fluentWait(By.id("iscat_"+st_desc[i]));
    cateAdd.click();
    test.get().pass("<small>[Checkbox]</small> Row "+st_desc[i]+" Set to Category");
    Thread.sleep(500);
}

```

# Row Counter

```JAVA

import java.util.List;

List<WebElement> rows = driver.findElements(By.xpath("//*[@id=\"tbl_quest\"]/tr"));
int count = rows.size();

```
##  Submit Button
### With Alert Check
```JAVA
Thread.sleep(500);
takeScreenShot(TC_ID, SC_TYPE, TC_ID);
test.get().addScreenCaptureFromPath(filePathSc + TC_ID + ".png");
Thread.sleep(500);
fluentWait(By.id("btn_a_2")).submit();
Thread.sleep(3000);
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
        Thread.sleep(3000);
    } else if(!alertval.contains("Successfully") && TEST_CASE_TYPE.equalsIgnoreCase("N")) {
        alert.accept();
        driver.switchTo().defaultContent();
        Thread.sleep(3000);
        driver.navigate().refresh();
        Thread.sleep(3000);
    } else {
        alert.accept();
        driver.navigate().refresh();
        Thread.sleep(3000);
        Assert.fail("Unexpected Alert Appeared. Test Case Type is "+ TEST_CASE_TYPE + " , but alert text is " + alertval);
    }
    Thread.sleep(4000);
}
```
### Without Alert Check
```JAVA
WebElement submit = fluentWait(By.id("btn_a_2"));
submit.click();
test.get().pass("<small>[Button]</small> Mengklik Submit");
Thread.sleep(4000);
//handle alert
takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_1"); // Report
test.get().pass("Submited", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_1.png").build());
resolveAllAlerts(driver, 16, true);	
Thread.sleep(4000);
```
---

##  Delete Button
```JAVA
driver.switchTo().parentFrame();
WebElement submit = fluentWait(By.id("btn_a_1"));
submit.click();
Thread.sleep(4000);
test.get().pass("<small>[Button]</small> Mengklik Delete");
//handle alert
resolveAllAlerts(driver, 16, true);
Thread.sleep(4000);
```


#   ScreenShoot & Close Second Window
> [Source](https://stackoverflow.com/questions/9588827/how-to-switch-to-the-new-browser-window-which-opens-after-click-on-the-button)

```JAVA
// Store the current window handle
String winHandleBefore = driver.getWindowHandle();

// Perform the click operation that opens new window
WebElement log = fluentWait(By.id("btn_a_1"));
log.click();
Thread.sleep(4000);
// Switch to new window opened
for(String winHandle : driver.getWindowHandles()){
    driver.switchTo().window(winHandle);
}

// Perform the actions on new window
takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_2"); // Report
test.get().pass("Menampilkan Log", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_2.png").build());

// Close the new window, if that window no more required
driver.close();
Thread.sleep(3000);
// Switch back to original browser (first window)
driver.switchTo().window(winHandleBefore);
```
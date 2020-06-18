Menu +[TASK](https://github.com/arshve/mardown/blob/master/Task.md)+ +[Repo Input](https://github.com/arshve/mardown/blob/master/Repo%20Input.md#Insert-Multiple-input-To-Right-Box)+ +[Repo Button](https://github.com/arshve/mardown/blob/master/Repo%20Button.md)+ +[Repo Documentation](https://github.com/arshve/mardown/blob/master/Repo%20Documentation.md)+ +[Repo Select By](https://github.com/arshve/mardown/blob/master/Repo%20Select%20By.md)+ +[Repo Select](https://github.com/arshve/mardown/blob/master/Repo%20Select.md)+ +[ModulSF List](https://github.com/arshve/mardown/blob/master/ModulSF6.md)+

# Hover Menu [Setting]

```JAVA
String homewindow = driver.getWindowHandle();
WebDriverWait wait = new WebDriverWait(driver, 120);
wait.until(ExpectedConditions.elementToBeClickable(By.xpath("//li[@id='menu_8']//a[@class='menulink']")));
WebElement menu = fluentWait(By.xpath("//li[@id='menu_11']//a[@class='menulink']")); // Setting
Actions actions = new Actions(driver);
actions.moveToElement(menu).perform();
Thread.sleep(500);
```

# Hover Child [Company]

```JAVA
WebElement submenu1 = fluentWait(By.linkText("Organization Setting")); // Organization Setting
Actions subactions1 = new Actions(driver);
subactions1.moveToElement(submenu1).perform();
Thread.sleep(500);
```

# Click Menu

```JAVA
JavascriptExecutor executor = (JavascriptExecutor) driver;
executor.executeScript("arguments[0].click();", submenu2);
checkPageIsReady();
Thread.sleep(5000);
```

# Click Add Button [Company]

```JAVA
wait.until(ExpectedConditions.frameToBeAvailableAndSwitchToIt(By.id("frmSFBody")));
Thread.sleep(5000);
fluentWait(By.id("ADD")).click(); // AddButton
Thread.sleep(5000);
test.get().pass("<small>[button]</small> Klik tombol Add");
driver.switchTo().parentFrame();
Thread.sleep(5000);
takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_1");
test.get().pass("Tampil Form Add Employee", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_1.png").build());
```

## Click Add Button 2 [Organization]

```JAVA
wait.until(ExpectedConditions.frameToBeAvailableAndSwitchToIt(By.id("frmSFBody")));
Thread.sleep(5000);

fluentWait(By.cssSelector("#form_toolbar > div.button-form.button.sprite-toolbar-add")).click();
Thread.sleep(5000);

test.get().pass("<small>[button]</small> Add <b>[+]</b> clicked, then Form Add Job Position Appeared");
driver.switchTo().parentFrame();
Thread.sleep(3000);
```

# Delete Handle [Company]

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

# Select Link With Attribute [Departement]

```JAVA
fluentWait(By.linkText(UNIT_CODE + ". " + UNIT_NAME)).click();
Thread.sleep(5000);
```

# SEARCH TARGET NAME

```JAVA
//			Search Course
WebElement search = fluentWait(By.id("header_ardata_1_3")); //Klik Subject
search.click();
Thread.sleep(1500);

WebElement searchname = fluentWait(By.id("txtSearch_3")); //Search Subject
searchname.sendKeys("");
searchname.sendKeys(Keys.HOME, Keys.chord(Keys.SHIFT, Keys.END), TARGET); //Mencari Subject sesuai xls
Thread.sleep(500);
searchname.sendKeys(Keys.ENTER); // Klik Enter
Thread.sleep(5000);

search.click();
Thread.sleep(1500);

test.get().pass("Mengisi data pencarian"); // Report
String searchnameval = searchname.getAttribute("value");
Assert.assertEquals(searchnameval, TARGET);
test.get().pass("<small>[Input Textfield]</small> Data Pencarian : " + searchnameval); // Report

WebElement linkno = fluentWait(By.linkText(TARGET)); //Klik Company Code
linkno.click();
Thread.sleep(3000);

takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_1"); // Report
test.get().pass("Menampilkan Form Update Training Course Form", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_1.png").build());
Thread.sleep(2000); // TimeOut

```

# Count Child Size

```JAVA
int xpathCount = driver.findElements(By.xpath("(//img[@title='Add'])")).size();
System.out.println(xpathCount);


```

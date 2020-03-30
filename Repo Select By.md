# Some Select By Method

#### By ID
```JAVA
WebElement [Variable] = fluentWait(By.id("[id]"));
```

#### By xPath
```JAVA
WebElement [Variable] = fluentWait(By.xpath("[xpath]"));
```

#### By Css Selector
```JAVA
WebElement [Variable] = fluentWait(By.cssSelector("[cssSelector]"));
```

#### Select Frame And Switch to It
```JAVA
wait.until(ExpectedConditions.frameToBeAvailableAndSwitchToIt(By.id("frmSFBody")));
```

#### Select object and wait until it clickable
```JAVA
wait.until(ExpectedConditions.elementToBeClickable(By.xpath("//li[@id='menu_8']//a[@class='menulink']")));
```

#### Checking isElement Exist
```JAVA
private boolean isElementPresent(By by) {
  try {
    driver.findElement(by);
    return true;
  } catch (NoSuchElementException e) {
    return false;
  }
}

boolean jr1 = isElementPresent(By.linkText("Something"));
```

#### Select All Item in element
```JAVA
java.util.List;

 Select oSelect = new Select(driver.findElement(By.id("yy_date_8")));
 List <WebElement> elementCount = oSelect.getOptions();
 int iSize = elementCount.size();
 
 for(int i =0; i<iSize ; i++){
 String sValue = elementCount.get(i).getText();
 System.out.println(sValue);
 }
```
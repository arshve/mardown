## Add Template

<details>
<summary> Add </summary>

```JAVA
package source.dataon.setting.payroll_setting.training_setting;
// source.dataon.setting.payroll_setting.training_setting.TAddTrainingCategory

import org.openqa.selenium.By;
import org.openqa.selenium.ElementNotVisibleException;
import org.openqa.selenium.JavascriptExecutor;
import org.openqa.selenium.Keys;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.interactions.Actions;
import org.openqa.selenium.support.ui.ExpectedConditions;
import org.openqa.selenium.support.ui.Select;
import org.openqa.selenium.support.ui.WebDriverWait;
import org.testng.Assert;
import org.testng.annotations.DataProvider;
import org.testng.annotations.Test;

import com.aventstack.extentreports.MediaEntityBuilder;
import com.aventstack.extentreports.markuputils.ExtentColor;
import com.aventstack.extentreports.markuputils.MarkupHelper;
import com.setup.BaseTest;
import com.setup.ReadExcel;

public class TAddTrainingCategory extends BaseTest {

    private static String file_location = curr + "//test-data//Add Training Category.xls";
    private static String sheet_name = "Test Data";

    private static ReadExcel re = new ReadExcel();


    @Test(dataProvider = "ReadData")
    public void TC_AddTrainingCategory(String TC_ID, String TEST_CASE_TYPE)
    		throws Exception {
    	String SC_TYPE = "vertical"; /*nonreport*/
    	String methodName = Thread.currentThread().getStackTrace()[1].getMethodName();
    	setTestName(driver.getCurrentUrl(), TC_ID, methodName, TEST_CASE_TYPE);
    	try {


    		//*************ADD COMPANY POLICY*************
    		checkPageIsReady();
            driver.switchTo().defaultContent();
            Thread.sleep(5000);

            // Select Setting
            WebDriverWait wait = new WebDriverWait(driver, 120);
            wait.until(ExpectedConditions.elementToBeClickable(By.xpath("//li[@id='menu_11']//a[@class='menulink']")));
            WebElement menu = fluentWait(By.xpath("//li[@id='menu_11']//a[@class='menulink']")); // Setting
            Actions actions = new Actions(driver);
            actions.moveToElement(menu).perform();
            Thread.sleep(1000);

            // Select Training Setting
            WebElement submenu1 = fluentWait(By.linkText("Training Setting")); // Training Setting
            Actions subactions1 = new Actions(driver);
            subactions1.moveToElement(submenu1).perform();
            Thread.sleep(1000);

            // Select Training Category
            WebElement submenu2 = fluentWait(By.linkText("Training Category")); // Training Category
            Actions subactions2 = new Actions(driver);
            subactions2.moveToElement(submenu2).perform();
            Thread.sleep(1000);

            // Click Job Title Menu
            JavascriptExecutor executor = (JavascriptExecutor) driver;
            executor.executeScript("arguments[0].click();", submenu2);
            checkPageIsReady();
            Thread.sleep(3000);
            test.get().pass(MarkupHelper.createLabel(">> Go to Setting > Training Setting > Training Category", ExtentColor.GREY));
            wait.until(ExpectedConditions.frameToBeAvailableAndSwitchToIt(By.id("frmSFBody")));

            Thread.sleep(5000);
            fluentWait(By.id("ADD")).click(); // AddButton
            Thread.sleep(5000);
            test.get().pass("<small>[button]</small> Add <b>[+]</b> clicked, then Form Add Job Title Appeared");
            driver.switchTo().parentFrame();
            Thread.sleep(3000);
            takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_1"); // Report
            test.get().pass("Add Company Policy Form", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_1.png").build());



            WebElement submit = fluentWait(By.id("btn_a_1"));
            submit.click();
            test.get().pass("<small>[Button]</small> Mengklik Submit");
            Thread.sleep(4000);
            //handle alert
            takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_1"); // Report
            test.get().pass("Submited", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_1.png").build());
            resolveAllAlerts(driver, 16, true);
            Thread.sleep(4000);

        } catch (ElementNotVisibleException e) {
            Assert.fail("Not Found Element/Page");
        }
    }

    @DataProvider(name = "ReadData")
    private static Object[][] readData() {
        Object[][] arrObject = re.getExcelData(file_location, sheet_name);
        return arrObject;
    }

}

```

</details>

## Edit Template

<details>
<summary> Edit </summary>

```JAVA

package source.dataon.setting.training_setting.training_instructor;

import org.openqa.selenium.By;
import org.openqa.selenium.ElementNotVisibleException;
import org.openqa.selenium.JavascriptExecutor;
import org.openqa.selenium.Keys;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.interactions.Actions;
import org.openqa.selenium.support.ui.ExpectedConditions;
import org.openqa.selenium.support.ui.Select;
import org.openqa.selenium.support.ui.WebDriverWait;
import org.testng.Assert;
import org.testng.annotations.DataProvider;
import org.testng.annotations.Test;

import com.aventstack.extentreports.MediaEntityBuilder;
import com.aventstack.extentreports.markuputils.ExtentColor;
import com.aventstack.extentreports.markuputils.MarkupHelper;
import com.setup.BaseTest;
import com.setup.ReadExcel;


public class TUpdateTrainingInstructor extends BaseTest {

	private static String file_location = curr + "//test-data//Update Training Instructor.xls";
	private static String sheet_name = "Test Data";

	private static ReadExcel re = new ReadExcel();


	@Test(dataProvider = "ReadData")
	public void TC_UpdateTrainingInstructor(
			String TC_ID, String CODE, String NAME, String PNAME, String TEST_CASE_TYPE)
			throws Exception {
		String SC_TYPE = "vertical"; /*nonreport*/
		String methodName = Thread.currentThread().getStackTrace()[1].getMethodName();
		setTestName(driver.getCurrentUrl(), TC_ID, methodName, TEST_CASE_TYPE);
		try {


			//*************ADD COMPANY POLICY*************
			checkPageIsReady();
            driver.switchTo().defaultContent();
            Thread.sleep(5000);

//			 Select Setting
            WebDriverWait wait = new WebDriverWait(driver, 120);
            wait.until(ExpectedConditions.elementToBeClickable(By.xpath("//li[@id='menu_11']//a[@class='menulink']")));
            WebElement menu = fluentWait(By.xpath("//li[@id='menu_11']//a[@class='menulink']")); // Setting
            Actions actions = new Actions(driver);
            actions.moveToElement(menu).perform();
            Thread.sleep(1000);

//	          Select Training Setting
            WebElement submenu1 = fluentWait(By.linkText("Training Setting")); // Training Setting
            Actions subactions1 = new Actions(driver);
            subactions1.moveToElement(submenu1).perform();
            Thread.sleep(1000);

//	          Select Training Category
            WebElement submenu2 = fluentWait(By.linkText("Training Instructor")); // Training Instructor
            Actions subactions2 = new Actions(driver);
            subactions2.moveToElement(submenu2).perform();
            Thread.sleep(1000);

//            Click Job Title Menu
            JavascriptExecutor executor = (JavascriptExecutor) driver;
            executor.executeScript("arguments[0].click();", submenu2);
            checkPageIsReady();
			Thread.sleep(3000);
			test.get().pass(MarkupHelper.createLabel(">> Go to Setting > Training Setting > Training Instructor", ExtentColor.GREY));
			wait.until(ExpectedConditions.frameToBeAvailableAndSwitchToIt(By.id("frmSFBody")));

//			 Search Target Name
			fluentWait(By.id("header_ardata_1_2")).click(); //Klik Subject
			Thread.sleep(1500);

			WebElement searchname = fluentWait(By.id("txtSearch_2")); //Search Subject
			searchname.sendKeys("");
			searchname.sendKeys(Keys.HOME, Keys.chord(Keys.SHIFT, Keys.END), NAME); //Mencari Subject sesuai xls
			Thread.sleep(500);

			searchname.sendKeys(Keys.ENTER); // Klik Enter
			Thread.sleep(5000);

			test.get().pass("Mengisi data pencarian"); // Report
			String searchnameval = searchname.getAttribute("value");
			Assert.assertEquals(searchnameval, NAME);
			test.get().pass("<small>[Input Textfield]</small> Data Pencarian : " + searchnameval); // Report
			WebElement linkno = fluentWait(By.linkText(CODE)); //Klik Company Code
			linkno.click();
			Thread.sleep(5000);

			test.get().pass("Mengklik Training Instructor Code :" + linkno.getText());// Report
			Thread.sleep(5000);

			driver.switchTo().parentFrame();
			Thread.sleep(5000);

			takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_1"); // Report
			test.get().pass("Menampilkan Form Training Instructor", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_1.png").build());

			WebElement submit = fluentWait(By.id("btn_a_2"));
			submit.click();
			test.get().pass("<small>[Button]</small> Mengklik Submit");
			Thread.sleep(4000);
			//handle alert
			takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_2"); // Report
			test.get().pass("Submited", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_2.png").build());
			resolveAllAlerts(driver, 16, true);
			Thread.sleep(4000);

		} catch (ElementNotVisibleException e) {
			Assert.fail("Not Found Element/Page");
		}
	}

	@DataProvider(name = "ReadData")
	private static Object[][] readData() {
		Object[][] arrObject = re.getExcelData(file_location, sheet_name);
		return arrObject;
	}
}
```

</details>

## Delete Template

<details>
<summary> Delete </summary>

```JAVA
package source.dataon.setting.training_setting.training_instructor;

import org.openqa.selenium.By;
import org.openqa.selenium.ElementNotVisibleException;
import org.openqa.selenium.JavascriptExecutor;
import org.openqa.selenium.Keys;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.interactions.Actions;
import org.openqa.selenium.support.ui.ExpectedConditions;
import org.openqa.selenium.support.ui.WebDriverWait;
import org.testng.Assert;
import org.testng.annotations.DataProvider;
import org.testng.annotations.Test;

import com.aventstack.extentreports.MediaEntityBuilder;
import com.aventstack.extentreports.markuputils.ExtentColor;
import com.aventstack.extentreports.markuputils.MarkupHelper;
import com.setup.BaseTest;
import com.setup.ReadExcel;


public class TDeleteTrainingInstructor extends BaseTest {

	private static String file_location = curr + "//test-data//Delete Training Instructor.xls";
	private static String sheet_name = "Test Data";

	private static ReadExcel re = new ReadExcel();


	@Test(dataProvider = "ReadData")
	public void TC_DeleteTrainingInstructor(
			String TC_ID, String CODE, String NAME, String TEST_CASE_TYPE)
			throws Exception {
		String SC_TYPE = "vertical"; /*nonreport*/
		String methodName = Thread.currentThread().getStackTrace()[1].getMethodName();
		setTestName(driver.getCurrentUrl(), TC_ID, methodName, TEST_CASE_TYPE);
		try {


			//*************ADD COMPANY POLICY*************
			checkPageIsReady();
            driver.switchTo().defaultContent();
            Thread.sleep(5000);

//			 Select Setting
            WebDriverWait wait = new WebDriverWait(driver, 120);
            wait.until(ExpectedConditions.elementToBeClickable(By.xpath("//li[@id='menu_11']//a[@class='menulink']")));
            WebElement menu = fluentWait(By.xpath("//li[@id='menu_11']//a[@class='menulink']")); // Setting
            Actions actions = new Actions(driver);
            actions.moveToElement(menu).perform();
            Thread.sleep(1000);

//	          Select Training Setting
            WebElement submenu1 = fluentWait(By.linkText("Training Setting")); // Training Setting
            Actions subactions1 = new Actions(driver);
            subactions1.moveToElement(submenu1).perform();
            Thread.sleep(1000);

//	          Select Training Category
            WebElement submenu2 = fluentWait(By.linkText("Training Instructor")); // Training Instructor
            Actions subactions2 = new Actions(driver);
            subactions2.moveToElement(submenu2).perform();
            Thread.sleep(1000);

//            Click Job Title Menu
            JavascriptExecutor executor = (JavascriptExecutor) driver;
            executor.executeScript("arguments[0].click();", submenu2);
            checkPageIsReady();
			Thread.sleep(3000);
			test.get().pass(MarkupHelper.createLabel(">> Go to Setting > Training Setting > Training Instructor", ExtentColor.GREY));
			wait.until(ExpectedConditions.frameToBeAvailableAndSwitchToIt(By.id("frmSFBody")));

//			 Search Target Name
			fluentWait(By.id("header_ardata_1_2")).click(); //Klik Subject
			Thread.sleep(1500);

			WebElement searchname = fluentWait(By.id("txtSearch_2")); //Search Subject
			searchname.sendKeys("");
			searchname.sendKeys(Keys.HOME, Keys.chord(Keys.SHIFT, Keys.END), NAME); //Mencari Subject sesuai xls
			Thread.sleep(500);

			searchname.sendKeys(Keys.ENTER); // Klik Enter
			Thread.sleep(5000);

			test.get().pass("Mengisi data pencarian"); // Report
			String searchnameval = searchname.getAttribute("value");
			Assert.assertEquals(searchnameval, NAME);
			test.get().pass("<small>[Input Textfield]</small> Data Pencarian : " + searchnameval); // Report
			WebElement linkno = fluentWait(By.linkText(CODE)); //Klik Company Code
			linkno.click();
			Thread.sleep(5000);

			test.get().pass("Mengklik Training Instructor Code :" + linkno.getText());// Report
			Thread.sleep(5000);

			driver.switchTo().parentFrame();
			Thread.sleep(5000);

			takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_1"); // Report
			test.get().pass("Menampilkan Form Training Instructor", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_1.png").build());


			WebElement submit = fluentWait(By.id("btn_a_1"));
			submit.click();
			test.get().pass("<small>[Button]</small> Mengklik Delete");
			Thread.sleep(4000);
			//handle alert
			takeScreenShot(TC_ID, SC_TYPE, TC_ID + "_2"); // Report
			test.get().pass("Deleted", MediaEntityBuilder.createScreenCaptureFromPath(filePathSc + TC_ID + "_2.png").build());
			resolveAllAlerts(driver, 16, true);
			Thread.sleep(4000);

		} catch (ElementNotVisibleException e) {
			Assert.fail("Not Found Element/Page");
		}
	}

	@DataProvider(name = "ReadData")
	private static Object[][] readData() {
		Object[][] arrObject = re.getExcelData(file_location, sheet_name);
		return arrObject;
	}
}
```

</details>

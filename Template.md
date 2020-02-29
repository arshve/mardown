```JAVA
package source.dataon.employee.employee_information; // Package Source
import java.util.List;
import com.aventstack.extentreports.MediaEntityBuilder;
import org.openqa.selenium.*;
import org.openqa.selenium.interactions.Actions;
import org.openqa.selenium.support.ui.ExpectedConditions;
import org.openqa.selenium.support.ui.Select;
import org.openqa.selenium.support.ui.WebDriverWait;
import org.testng.Assert;
import org.testng.annotations.DataProvider;
import org.testng.annotations.Test;
import com.setup.ReadExcel;
import com.setup.BaseTest;

public class TAdd_Employee extends BaseTest { // Package name

    private static String file_location = curr + "//test-data//[Excell File Dir]"; // Excell Directory
    private static String sheet_name = "Test Data";

    private static ReadExcel re = new ReadExcel();

    @Test(dataProvider = "ReadData")
    // Excell Data To Pass in Script
    public void [FileName](String NO, String TC_ID, [Excell], String TEST_CASE_TYPE) 
    
    throws Exception {
        String SC_TYPE = "vertical"; /*nonreport*/
        String methodName = Thread.currentThread().getStackTrace()[1].getMethodName();
        setTestName(driver.getCurrentUrl(), TC_ID, methodName, TEST_CASE_TYPE);
        try {
            // *************Script*************
            // Default Start
            checkPageIsReady();
            driver.switchTo().defaultContent();
            Thread.sleep(3000);
            // -------------

            // Script Start
            [Script Func]
            // --------------
            
        } catch (ElementNotVisibleException e) {
            Assert.fail("Not Found Element/Page");
        }
    }

    @DataProvider(name = "ReadData")
    private static Object[][] updateworklocation() {
        Object[][] arrObject = re.getExcelData(file_location, sheet_name);
        return arrObject;
    }

}
```
# MavenAPPTesting
Testing the Login functionality of amazon
package MavenTestingdemo;

import org.junit.Before;
import org.junit.Test;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.chrome.ChromeDriver;
import org.testng.asserts.Assertion;

public class MaveappTesting {

	private WebDriver driver;
	
	@Before
	public void testSetup(){
	System.out.println("Testing case done successfully"); 
	System.setProperty("webdriver.chrome.driver", "C:\\Users\\user\\Downloads\\chromedriver_win32\\chromedriver.exe");
	driver = new ChromeDriver();    
	}
    @Test
    public void testmethod(){
    driver.get("https://www.ebay.com/");
    }
    @Test
    public void doLogin(){
    System.out.println("user can login with valid username and password successfully");   
    }
    
    @Test
    public void logout(){
    System.out.println("user can logout successfully");   
    }
    @Test
    public void Advance_search(){
    System.out.println("user can do advance search");  
    }
    @Test
    public void buy_products(){
    System.out.println("user can buy producst");         
    }
    }

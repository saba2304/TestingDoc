# TestingDoc


import org.openqa.selenium.*;

public class AutomationPractice_com {

	public static void main(String[] args) {
		
		System.setProperty("webdriver.gecko.driver",
				"C:\\geckodriver\\geckodriver.exe");

		
		WebDriver driver = new FirefoxDriver();
		//Puts an Implicit wait, Will wait for 10 seconds before throwing exception
		driver.manage().timeouts().implicitlyWait(10, TimeUnit.SECONDS);
		
		//Launch website
		driver.navigate().to("http://automationpractice.com/index.php");
		
		//Maximize the browser
	     driver.manage().window().maximize();
	     
	    // click sign button
	      driver.findElement(By.xpath("/html/body/div/div[1]/header/div[2]/div/div/nav/div[1]/a")).click();
	      
	    // wait for 5 seconds  
	      try {
				Thread.sleep(10000);
			} catch (InterruptedException e) {
				e.printStackTrace();
			}
	      
	    // Enter e-mail address
	      driver.findElement(By.xpath("//*[@id=\"email_create\"]")).sendKeys("z1234667@gmail.com");
	      
	      try {
				Thread.sleep(5000);
			} catch (InterruptedException e) {
				e.printStackTrace();
			}
	      
	      //click on create account
	      driver.findElement(By.xpath("//*[@id=\"SubmitCreate\"]")).click();
	      
	      try {
				Thread.sleep(5000);
			} catch (InterruptedException e) {
				e.printStackTrace();
			}
	      
	     // click on title
	      driver.findElement(By.xpath("//*[@id=\"id_gender2\"]")).click();
	      
	     //Enter first name
	      driver.findElement(By.xpath(" //*[@id=\"customer_firstname\"]")).sendKeys("saba");
	      
	      //Enter last name
	      driver.findElement(By.xpath("//*[@id=\"customer_lastname\"]")).sendKeys("Anjum");
	      
	    //Enter password
	      driver.findElement(By.xpath("//*[@id=\"passwd\"]")).sendKeys("abcdefg");
	    
	      //Enter date of birth
	      
	      //Enter address 
	      //Enter first name
	      driver.findElement(By.xpath("//*[@id=\"firstname\"]")).sendKeys("saba");
	      
	      //Enter lastname
	      driver.findElement(By.xpath("  //*[@id=\"lastname\"]")).sendKeys("Anjum");
	     
	      // Enter company
	      driver.findElement(By.xpath("//*[@id=\"company\"]")).sendKeys("Xpedia");
	      
	      // Enter address
	      driver.findElement(By.xpath("//*[@id=\"address1\"]")).sendKeys("Gurgaon");
	      
	      // Enter city
	      driver.findElement(By.xpath("//*[@id=\"city\"]")).sendKeys("New Delhi");
	      
	      // Enter state
	      Select dropdown = new Select(driver.findElement(By.xpath("//*[@id=\"id_state\"]")));
	      
	      dropdown.selectByVisibleText("Iowa");
	      
	      // Enter zip
	      driver.findElement(By.xpath(" //*[@id=\"postcode\"]")).sendKeys("48700");
	      
	      // Enter country
	      driver.findElement(By.xpath(" //*[@id=\"id_country\"]")).sendKeys("United states");
	      
	      // Enter mobile_phone
	      driver.findElement(By.xpath(" //*[@id=\"phone_mobile\"]")).sendKeys("8932014476");
	      
	      //click on register
	      driver.findElement(By.xpath("//*[@id=\"submitAccount\"]")).click();
	      
	   // wait for 5 seconds  
	      driver.manage().timeouts().implicitlyWait(15, TimeUnit.SECONDS);
	      
	    //click on dress
	      driver.findElement(By.xpath("/html/body/div/div[1]/header/div[3]/div/div/div[6]/ul/li[2]/a")).click();
	      // wait for 5 seconds  
	      try {
				Thread.sleep(5000);
			} catch (InterruptedException e) {
				e.printStackTrace();
			}
	      
	      //click on selected dress 
	      driver.findElement(By.xpath("/html/body/div/div[2]/div/div[3]/div[2]/ul/li[2]/div/div[1]/div/a[1]/img")).click();
	      // wait for 5 seconds  
	      try {
				Thread.sleep(5000);
			} catch (InterruptedException e) {
				e.printStackTrace();
			}
	      
	      //add to cart
	      driver.findElement(By.xpath("/html/body/div/div[2]/div/div[3]/div/div/div/div[4]/form/div/div[3]/div[1]/p/button")).click();
	     
	      
	      //proceed to check out
	      driver.findElement(By.xpath("/html/body/div/div[1]/header/div[3]/div/div/div[4]/div[1]/div[2]/div[4]/a")).click();
	      
	      // wait for 5 seconds  
	      try {
				Thread.sleep(5000);
			} catch (InterruptedException e) {
				e.printStackTrace();
			}
	      //proceed to check out
	      driver.findElement(By.xpath("/html/body/div/div[2]/div/div[3]/div/p[2]/a[1]")).click();
	      
	      // Thanks
	      driver.findElement(By.xpath("/html/body/div/div[2]/div/div[3]/div/form/div/div[3]/textarea")).sendKeys("Nice Shopping");
	      
	      // proceed to check out
	      driver.findElement(By.xpath("/html/body/div/div[2]/div/div[3]/div/form/p/button")).click();
	      
	      try {
				Thread.sleep(5000);
			} catch (InterruptedException e) {
				e.printStackTrace();
			}
	      
	      // tick on terms and conditions
	      driver.findElement(By.xpath("//*[@id=\"cgv\"]")).click();
	      try {
				Thread.sleep(5000);
			} catch (InterruptedException e) {
				e.printStackTrace();
			}
	      
	      //proceed to checkout
	      driver.findElement(By.xpath("/html/body/div/div[2]/div/div[3]/div/div/form/p/button")).click();
	      try {
				Thread.sleep(5000);
			} catch (InterruptedException e) {
				e.printStackTrace();
			}
	      
	      System.out.println(" shopping done ");
	      
	    //Close the Browser.
	      driver.close();
	      
	      
	      
	    }

}

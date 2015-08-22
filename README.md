# arvinth
package testing;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.firefox.FirefoxDriver;

public class Selenium {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		WebDriver driver=new FirefoxDriver();
		driver.get("https://edit.europe.yahoo.com/registration");
		driver.manage().window().maximize();
		driver.findElement(By.id("first-name")).sendKeys("B");
		driver.findElement(By.id("last-name")).sendKeys("Aravindhan");
		driver.findElement(By.id("user-name")).sendKeys("91aravind");
		driver.findElement(By.id("password")).sendKeys("binga");
		driver.findElement(By.id("mobile")).sendKeys("9942969403");
		driver.findElement(By.id("male")).click();
		driver.findElement(By.id("mobile-rec")).sendKeys("9942969403");
		driver.findElement(By.id("relationship")).sendKeys("BRO");
		driver.findElement(By.className("button submit btn-purple")).click();
		driver.close();
		
	}

}

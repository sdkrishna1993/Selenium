# DropDown
#Print all the texts appear inside the dropdown list
Select dropDown = new Select(driver.findElement(By.id("userRegistrationForm:security")));
	            List <WebElement> elementCount = dropDown.getOptions();
	            int itemSize = elementCount.size();
	            for(int i = 0; i < itemSize ; i++){
	                String optionsValue = elementCount.get(i).getText();
	                System.out.println(optionsValue);

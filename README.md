# AutomationTest

**PREREQUISITES**
Ensure you have the following installed:

1.) An IDE of your choice (e.g. IntelliJ or Eclipse)

2.) Import the JUnit library into your IDE

3.) Ensure you have the latest Java JDK installed (http://www.oracle.com/technetwork/java/javase/downloads/index.html)

4.) Ensure you have the latest Selenium Java Drivers installed (http://www.seleniumhq.org/download/)

5.) Download the Chrome Driver (https://sites.google.com/a/chromium.org/chromedriver/)

Now please download the project and import it into your IDE then simply run the classes called "WikipediaTests" and "TravelexTests". =)

Thanks!


**Design Choices**
One of the most important design choices that I have chosen to use within my test scripts is the Page Object Model. I used this for the Travelex and Wikipedia homepages as every test is to hit these pages before it begins. Due to the nature of the task set being so small, I was not able to create too many Page Object Models (POM) - however if there were other tests that required reusable code e.g. logging a user in, then a PAge Object Model would have been used for this.
The reason I use Page Object Models is because first and foremost it makes the code cleaner and easier to understand. POM also means low maintenance, for example if I need to change the URL that each test case is hitting, I will only need to change it in one location. For massive test suites this can prove extremely time effective as you will not need to modify over 100 test cases.

I also choose to implement JUnit within my test cases which proves extremely beneficial as it acts as essentially a "second line of defence". It allows me to verify/assert a response that may not be part of the GUI and therefore hard or impossible for the human eye to catch. Selenium WebDriver is essentially a lot of UI testing so anything in the "backend" or anything that needs to be verified which would be a tedious job for a tester can easily be done with Unit Tests. They also help to catch bugs/issues early in the code and thus minimalizing the impact.

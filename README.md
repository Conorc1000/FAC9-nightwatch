# FAC9-nightwatch

### FAC9 learn nightwatch tutorial

#### What is nightwatch and how does it work

 - [nightwatch.js.org](http://nightwatchjs.org/)
 - Nightwatch is an end to end testing framework
 - You can write tests with it, these tests will click through the application on the browser and make assertions about what is displayed on the page.
 - The syntax is very readable to anyone who can understand js html and css eg;
  
      .url('http://www.google.com')
      .waitForElementVisible('body', 1000)
      .assert.title('Google')
      .assert.visible('input[type=text]')
      .setValue('input[type=text]', 'rembrandt van rijn')
      .waitForElementVisible('button[name=btnG]', 1000)
      .click('button[name=btnG]')

 - It works by looking at an application which is being served, either on your local host or somewhere like heroku. 
The application is then opened on either a browser on your device [show example] or you can ask for the tests to be run on any of the available sauce labs devices.

##### Key word:
  - Selenium chromeDriver = An API which we install, it allows us to control the browser using our test scripts.

#### Task1 (45mins): 
Get into you groups from last week and set up night watch test to run on you local devices. Use the DWYL learn nightwatch readme. You will be presenting your tests at he end. Bonus: Set up the tests to take screen shots at certain points.
Do the initial setup of the night watch.con.js chrome driver together.
you can choose whether you have to manually run "node nightwatch.conf.js” or you can set it as a post install command, I would recommend the second.

##### Key word:
 -  SauceLabs = Gives us access to a vast range of browsers and devices to test the application on. Offers us an interface to see recordings of our automated test. Also allows to to manually click through you application while it is being run on another device.


#### Task2 (45mins): 
Now make these same tests pass remotely using sauce labs, this will involve setting up sauce labs connect I would recommend using the fire fox plugin. [show example]

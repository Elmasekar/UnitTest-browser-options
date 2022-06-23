# How to set browser specific options in UnitTest on [LambdaTest](https://www.lambdatest.com/?utm_source=github&utm_medium=repo&utm_campaign=UnitTest-browser-options)

If you want to set browser specific options for an automation test in UnitTest on Lambdatest, you can use the following steps. You can refer to sample test repo [here](https://github.com/LambdaTest/UnitTest-browser-options).

# Steps:

You can specify the various browser specific options in the test file capabilities. The following is an example on how to set Chrome specific options using chromeOptions:

```python
desired_caps = {
            'LT:Options': {
                "build": "Python Demo",  # Change your build name here
                "name": "Python Demo Test",  # Change your test name here
                "platformName": "Windows 11",
                "selenium_version": "4.0.0",
                "chromeOptions" : {
                "args" : ["incognito"]  # ChromeOption to start chrome in incognito mode
                
            },
            "browserName": "Chrome",
            "browserVersion": "98.0",
        }

```

* The different options available for Chrome can be referred to [here](https://seleniumhq.github.io/selenium/docs/api/py/webdriver_chrome/selenium.webdriver.chrome.options.html).

* For more information you can refer to this LambdaTest [blog](https://www.lambdatest.com/blog/desired-capabilities-in-selenium-testing/?utm_source=github&utm_medium=repo&utm_campaign=Pytest-browser-options).


## Run your test

```bash
python lambdatest.py
```

# Links:

[LambdaTest Community](http://community.lambdatest.com/)

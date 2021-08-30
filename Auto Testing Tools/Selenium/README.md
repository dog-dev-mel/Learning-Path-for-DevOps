# Selenium

## What is Selenium ?

Selenium [səˈliːniəm] is a Web UI automated test suites, which supports across different browsers, platforms and programming languages including C#, Java, Perl, PHP, Python and Ruby.
It can work with Ant, Maven, Jenkins and Docker for the CI/CD tasks as well as integrate with TestNG or Junit for generate testing report.

## Limitation

- It cannot support WEB services automation such as SOAP or REST

- It needs to use a specific programming language to write scripts running in the Selenium WebDriver.

- It uses Page Object Model to store and maintain objects rather than build-in objects in UTF/QTP.

- It needs to work with Sikuli to support the requirement of Image testing.

## Selenium Suite

- Selenium IDE(Plugins): It record all actions/interactions between users and browsers and then automated to generate javascript-based testing scripts. It also can convert it to other programming languages.

  It supports six ways to locate a design WEB elements, which are **by Name, by Xpath, by CSS, by DOM, by ID Element or by Identifier.**

  Currently, it only supports Firefox and Chrome.

- Selenium WebDriver:It applies scripts on WebDriver Client libraries to communicate with Web Browser. This way is more quick than Selenium RC using a mid-server/proxy to connect with Web Browser.

    It can support mobile applications.

    It can supports some advanced web elements such as pull-down list，check box and waring.

    It supports IE, Firefox, Chrome, Safari, Opera and so on.

- Selenium Grid: It can run scripts on multiple machines.

### Selenium WebDriver Installation

1. Installing Selenium libraries:
    Python: pip install selenium

2. Installing browser drivers:
    - export PATH=$PATH:/opt/WebDriver/bin >> ~/.profile
    - Download the matched geckodriver in the folder
    - geckodriver (Chrome will crash Intel lake chips or Ubuntu.)

    - (base) ****@HINGE:/opt/WebDriver$ geckodriver
     1630321035981	geckodriver	INFO Listening on 127.0.0.1:4444
    - Alternative 终极大招：也可以直接sudo apt-get install firefox-geckodriver
    - geckodriver

3. Create a python file

    **#Simple assignment**

    from selenium.webdriver import Firefox

    driver = Firefox()

    **#Or use the context manager**

    from selenium.webdriver import Firefox

    Firefox(executable_path='/path/to/geckodriver') #如果使用apt-get安装geckodriver可以省略此步骤
  
    with Firefox() as driver:

      **#your code inside this indent**
      driver.get("https://selenium.dev")

    **总结**，首先使用apt安装webdriver，此方法可以自动添加到路径中，使用命令行直接调用测试，

    其次，选择对应语言安装对应的selenium的package，

    最周，脚本中直接调用即可，不需指定路径。
  
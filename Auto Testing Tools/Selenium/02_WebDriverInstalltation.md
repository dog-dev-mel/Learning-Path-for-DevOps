## 2. Selenium WebDriver Installation

WebDriver is a remote control **interface** that enables introspection and control of user agents.

**Local Model:**

WebDriver(Bindings+Support classes)======**Driver(ChromeDriver/GeckoDriver)======Browser**

**Remote Single node Model:**

WebDriver(Bindings+Support classes)======**Remote WebDriver======Driver(ChromeDriver/GeckoDriver)======Browser**

**Remote Distributed computing Model**：

WebDriver(Bindings+Support classes)======Selenium Server or Grid======**Driver(ChromeDriver/GeckoDriver)======Browser**

**!!!!!!Note**:
HOST SYSTEM will be composed of components in overstriking words.


### Installing Steps:

1. Installing Selenium libraries:
    Python: pip install selenium

2. Installing browser drivers:
    - export PATH=$PATH:/opt/WebDriver/bin >> ~/.profile
    - Download the matched geckodriver in the folder
    - geckodriver (Chrome will crash Intel lake chips or Ubuntu.)

    - (base) ****@HINGE:/opt/WebDriver$ geckodriver
     1630321035981 geckodriver INFO Listening on 127.0.0.1:4444
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
  
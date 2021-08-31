# Selenium

## 1. What is Selenium ?

Selenium [səˈliːniəm] is a Web UI automated test suites, which supports across different browsers, platforms and programming languages including C#, Java, Perl, PHP, Python and Ruby.
It can work with Ant, Maven, Jenkins and Docker for the CI/CD tasks as well as integrate with TestNG or Junit for generate testing report.

### Limitation

- It cannot support WEB services automation such as SOAP or REST

- It needs to use a specific programming language to write scripts running in the Selenium WebDriver.

- It uses Page Object Model to store and maintain objects rather than build-in objects in UTF/QTP.

- It needs to work with Sikuli to support the requirement of Image testing.

### Selenium Suite

- Selenium IDE(Plugins): It record all actions/interactions between users and browsers and then automated to generate javascript-based testing scripts. It also can convert it to other programming languages.

  It supports six ways to locate a design WEB elements, which are **by Name, by Xpath, by CSS, by DOM, by ID Element or by Identifier.**

  Currently, it only supports Firefox and Chrome.

- Selenium WebDriver:It applies scripts on WebDriver Client libraries to communicate with Web Browser. This way is more quick than Selenium RC using a mid-server/proxy to connect with Web Browser.

    It can support mobile applications.

    It can supports some advanced web elements such as pull-down list，check box and waring.

    It supports IE, Firefox, Chrome, Safari, Opera and so on.

- Selenium Grid: It can run scripts on multiple machines.

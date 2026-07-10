# Simple Selenium Example

A small Java 17, Maven, Selenium and TestNG project based on the idea of
`llanni/minimalseleniumproject`.

The test opens SauceDemo, signs in with the site's public demonstration account,
and verifies that the **Products** page appears.

## Requirements

- Java 17 or newer
- Maven
- Google Chrome
- Internet access

Selenium Manager is built into Selenium, so you do not need to manually download
or configure ChromeDriver.

## Run locally

Normal browser mode:

```bash
mvn clean test
```

Headless mode:

```bash
mvn clean test -Dheadless=true
```

Test reports are created under:

```text
target/surefire-reports/
```

## Project structure

```text
Simple-Selenium-Example/
├── .github/workflows/selenium-tests.yml
├── src/test/java/tests/LoginBasicTest.java
├── .gitignore
├── pom.xml
├── README.md
└── testng.xml
```


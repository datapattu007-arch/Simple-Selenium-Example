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

## Upload to GitHub

Create an empty repository named `Simple-Selenium-Example`. Do not add a README,
.gitignore, or licence in GitHub because these files are already included here.

Open Git Bash or a terminal inside this project folder and run:

```bash
git init
git branch -M main
git add .
git commit -m "Add simple Selenium TestNG project"
git remote add origin https://github.com/YOUR_USERNAME/Simple-Selenium-Example.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.

After pushing, open the repository's **Actions** tab. The `Selenium Tests`
workflow should run automatically. You can also open it and choose
**Run workflow**.

## Connect to Ordino

1. Create an Ordino automation project.
2. Select GitHub and GitHub Actions.
3. Connect the GitHub account containing this repository.
4. Grant read access to `Simple-Selenium-Example`.
5. Return to Ordino and select **Check access again**.
6. Continue to the project after GitHub access is confirmed.

Note: this is a Selenium/TestNG repository. Do not label it as Playwright unless
Ordino currently supports only Playwright and you intentionally want to convert it.

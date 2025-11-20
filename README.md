# selenium-auto-base

This project is a basic Selenium automation framework built with **Java**, **Maven**, and **TestNG**.  
It’s mainly for practicing UI automation concepts such as element interaction, navigation, assertions, and simple test structuring.

---

## 🧱 Project Structure

```
SeleniumProject2/
├── src/
│ ├── test/java/ → Test classes
│ ├── main/java/ → Reusable helpers / utilities
├── testng-suites/
│ └── testng.xml → Main TestNG suite executed by Maven Surefire
├── pom.xml
```
---

## ⚙️ Tech Stack

- **Java 1.8**
- **Selenium WebDriver 2.53.1**  
- **TestNG 6.9.10**
- **Maven Surefire Plugin**
- **Apache POI** (Excel handling)
- **ReportNG** (HTML report plugin)

> Note: Selenium 2.x is very old. Upgrading to Selenium 4 later

---

## 🧪 How Tests Run

Maven Surefire is configured to:

- Run TestNG through `testng-suites/testng.xml`
- Detect test classes automatically (`*Test.java`, `*Tests.java`, `Test*.java`, etc.)
- Generate reports under: test-reports/

---

## ▶️ How to Execute

### **Run from terminal**
```bash
mvn clean test
Run a specific TestNG suite
bash
Copy code
mvn clean test -DsuiteXmlFile=testng-suites/testng.xml
```
### **Run from IDE**
Open the project in IntelliJ/Eclipse

Right-click any test class → Run

or run the TestNG suite XML directly

---
## **📦 Dependencies Overview**
Key libraries configured in pom.xml:
- Selenium WebDriver
- HtmlUnit Driver
- TestNG
- Apache HttpClient (for API/HTTP calls)
- Apache POI (Excel read/write)
- ReportNG (TestNG reporting plugin)

---

## **📝 Purpose of This Project**
This repo is mainly for learning:

- Writing basic Selenium scripts
- Understanding locators (id/xpath/css)
- Running tests with TestNG suites
- Organizing code for UI automation
- Handling simple reports and Excel data

---

## **🚀 Future Improvements**
- Add Page Object Model (POM)
- Add logging (SLF4J + Log4j2)
- Add WebDriverManager
- Use a modern test report (Allure)

# 🚀 Selenium WebDriver Automation Framework (Java)  

[![Java](https://img.shields.io/badge/Java-17%2B-orange?logo=openjdk)](https://www.java.com/)
[![Selenium](https://img.shields.io/badge/Selenium-4.0%2B-brightgreen?logo=selenium)](https://selenium.dev)
[![Maven](https://img.shields.io/badge/Maven-3.8%2B-blue?logo=apachemaven)](https://maven.apache.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A robust **Java-based Selenium WebDriver** framework for automated web testing, designed for reliability and ease of use. Includes examples for common web interactions, best practices, and scalable test structure.

---

## 📌 Table of Contents  
- [Features](#-features)  
- [Prerequisites](#-prerequisites)  
- [Setup Guide](#%EF%B8%8F-setup-guide)  
- [Running Tests](#-running-tests)  
- [Project Structure](#-project-structure)  
- [Best Practices](#%EF%B8%8F-best-practices)  
- [Contributing](#-contributing)  
- [License](#-license)  

---

## 🌟 Features  
✔ **Cross-Browser Testing**: Chrome, Firefox, Edge support  
✔ **Page Object Model (POM)**: Maintainable and reusable code  
✔ **Maven Integration**: Dependency management made easy  
✔ **Sample Tests**: Forms, dynamic elements, waits, and assertions  
✔ **Configurable**: Centralized properties for URLs/drivers  

---

## 📦 Prerequisites  
Ensure you have the following installed:  
- **Java JDK 17+** ([Download](https://adoptium.net/))  
- **Maven 3.8+** ([Guide](https://maven.apache.org/install.html))  
- **Browser Drivers**:  
  - [ChromeDriver](https://chromedriver.chromium.org/)  
  - [GeckoDriver (Firefox)](https://github.com/mozilla/geckodriver)  

---

## ⚙️ Setup Guide  

### 1. Clone the Repository  
```bash
git clone https://github.com/chowdhury-nahid/webdriver_java.git
cd webdriver_java
```

### 2. Configure Drivers  
Place downloaded drivers in:  
```
src/main/resources/drivers/
```  
Update paths in `config.properties`:  
```properties
# Example:
chrome.driver.path=src/main/resources/drivers/chromedriver.exe
```

### 3. Build Dependencies  
```bash
mvn clean install
```

---

## 🧪 Running Tests  
### Run All Tests  
```bash
mvn test
```

### Run a Specific Test Class  
```bash
mvn test -Dtest=BaseTest
```

### IDE Execution  
Import as a **Maven project** in IntelliJ/Eclipse and run via JUnit.  

---

## 📂 Project Structure  
```plaintext
webdriver_java/
├── src/
│   ├── main/java/
│   │   ├── pages/           # Page Object Classes
│   │   ├── utils/           # Helpers (e.g., WebDriverManager)
│   │   └── BaseTest.java    # Test Base Class
│   ├── test/java/           # Test Scripts
│   └── resources/
│       ├── drivers/         # Browser Drivers
│       └── config.properties
├── pom.xml                 # Maven Dependencies
└── README.md
```

---

## 🛠️ Best Practices  
✅ **Page Object Model (POM)**: Separates UI mapping from test logic.  
✅ **Explicit Waits**: Avoids flaky tests with `WebDriverWait`.  
✅ **Singleton WebDriver**: Ensures single driver instance per session.  
✅ **Logging**: Integrate Log4j for execution traces.  

---

## 🤝 Contributing  
1. Fork the repository.  
2. Create a branch (`git checkout -b feature/your-feature`).  
3. Commit changes (`git commit -m 'Add feature'`).  
4. Push to the branch (`git push origin feature/your-feature`).  
5. Open a **Pull Request**.  

---

## 📜 License  
Distributed under the **MIT License**. See [LICENSE](LICENSE) for details.  

---

## 📬 Contact  
**Nahid Chowdhury**  
- GitHub: [@chowdhury-nahid](https://github.com/chowdhury-nahid)  
- LinkedIn: [Nahid Chowdhury](https://www.linkedin.com/in/chowdhury-nahid/)  

```

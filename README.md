# Playwright TypeScript Automation Framework

A web automation testing framework built using **Playwright, TypeScript, and the Page Object Model (POM)** design pattern.

## 📁 Project Structure

```text
Chit-Playwright-JS-FW/
│
├── pages/
│   ├── CartPage.ts
│   ├── CheckoutPage.ts
│   ├── HomePage.ts
│   ├── LoginPage.ts
│   ├── PaymentPage.ts
│   └── ProductPage.ts
│
├── test-data/
│   └── testData.json
│
├── tests/
│   ├── addproducttocart.spec.ts
│   ├── home.spec.ts
│   ├── login.spec.ts
│   └── purchase.e2e.spec.ts
│
├── .gitignore
└── README.md
```

## 🚀 About the Project

This project is designed to automate web application testing using Playwright with TypeScript.

The framework follows the Page Object Model (POM) architecture to maintain reusable page classes, separate test scenarios, and organized test data.

### Key Features

- Playwright Test for browser automation.
- TypeScript for type-safe test development.
- Page Object Model (POM) architecture.
- Reusable page classes and methods.
- External JSON test data management.
- End-to-end testing of application workflows.
- Automated login and product-related test scenarios.
- Easy maintenance and scalability.

## 🛠️ Technologies Used

- Playwright
- TypeScript
- Node.js
- npm
- Visual Studio Code

## 📋 Prerequisites

Make sure the following are installed:

- Node.js
- npm
- Visual Studio Code
- Git

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone <repository-url>
```

### 2. Navigate to the Project

```bash
cd Chit-Playwright-JS-FW
```

### 3. Install Dependencies

```bash
npm install
```

### 4. Install Playwright Browsers

```bash
npx playwright install
```

## 🏗️ Framework Architecture

### 1. Pages

The `pages` folder contains reusable page classes following the Page Object Model.

Each page class contains page-specific locators and methods.

| Page Class | Description |
|---|---|
| HomePage.ts | Handles homepage navigation and login/signup navigation. |
| LoginPage.ts | Handles login functionality. |
| ProductPage.ts | Handles product navigation and add-to-cart functionality. |
| CartPage.ts | Handles cart interactions and validations. |
| CheckoutPage.ts | Handles checkout functionality. |
| PaymentPage.ts | Handles payment-related functionality. |

### 2. Test Data

The `test-data` folder contains test data used by automation scripts.

**File:**

`test-data/testData.json`

It contains test inputs such as:

- Login email
- Login password
- Product details
- Other test-related data

Test data is imported into test files to avoid hardcoding values.

### 3. Tests

The `tests` folder contains Playwright test scenarios.

| Test File | Description |
|---|---|
| home.spec.ts | Tests homepage functionality. |
| login.spec.ts | Tests login functionality. |
| addproducttocart.spec.ts | Tests adding products to the shopping cart. |
| purchase.e2e.spec.ts | Tests the complete purchase workflow. |

## 🧪 Test Scenarios

### Home Page Testing

- Verify homepage navigation.
- Verify homepage functionality.
- Verify navigation to login/signup.

### Login Testing

- Verify login functionality.
- Verify login with valid credentials.
- Verify successful authentication.

### Add Product to Cart

- Navigate to the application.
- Open the login page.
- Login using test credentials.
- Navigate to products.
- Select a product.
- Add the product to the cart.

### Purchase End-to-End Testing

- Login to the application.
- Navigate to products.
- Add products to the cart.
- Proceed to checkout.
- Complete the purchase workflow.
- Verify the order confirmation.

## ▶️ Running Tests

### Run All Tests

```bash
npx playwright test
```

### Run a Specific Test File

```bash
npx playwright test tests/home.spec.ts
```

### Run Login Test

```bash
npx playwright test tests/login.spec.ts
```

### Run Add Product to Cart Test

```bash
npx playwright test tests/addproducttocart.spec.ts
```

### Run Purchase Test

```bash
npx playwright test tests/purchase.e2e.spec.ts
```

### Run Tests in Headed Mode

```bash
npx playwright test --headed
```

### Run a Specific Test File in Headed Mode

```bash
npx playwright test tests/addproducttocart.spec.ts --headed
```

### Run Tests in Chromium

```bash
npx playwright test --project=chromium
```

Use the browser project name configured in your Playwright configuration.

## 📊 Test Reports

Playwright provides HTML reports to review test execution results.

### Generate and View Report

```bash
npx playwright test
```

```bash
npx playwright show-report
```

The report helps identify:

- Passed test cases
- Failed test cases
- Execution details
- Error messages
- Test execution status

## 🔄 Framework Workflow

1. Open the application.
2. Navigate to the required page.
3. Perform actions using page class methods.
4. Execute test scenarios.
5. Validate expected results.
6. Generate and review test reports.

## 📝 Best Practices

- Follow the Page Object Model.
- Keep page locators and methods inside page classes.
- Maintain test data separately.
- Use reusable methods for common actions.
- Keep test scenarios independent.
- Use meaningful test names.
- Avoid hardcoding sensitive credentials.
- Review test reports after execution.
- Maintain clean and readable code.

## 🐛 Troubleshooting

### Browser Not Installed

Run:

```bash
npx playwright install
```

### Test Not Found

Verify the test file path and filename.

### Application Not Opening

Check the application URL and internet connection.

### Test Data Error

Verify the JSON file path and syntax.

### Browser Project Error

Verify the browser project name in the Playwright configuration.

## 👩‍💻 Author

Playwright TypeScript Automation Framework


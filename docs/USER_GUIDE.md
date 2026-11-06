# SpendWise — User Guide

## 1. Opening the website

1. Open the SpendWise project folder in Visual Studio Code.
2. Open `index.html` with Live Server, or open the file directly in a browser.
3. Use the navigation bar to move between pages.

## 2. Website pages

### Home
Introduces SpendWise and displays illustrative financial summary information. Use the dashboard link to view the example dashboard.

### About
Describes the purpose, objectives, and intended value of the project.

### Dashboard
Displays example total balance, income, expenses, savings, category summaries, and recent activity. Values are static sample data.

### Add Expense
Shows fields for entering an expense title, amount, date, category, payment method, and description. The amount field is labeled `Amount` and uses an `Rs.` prefix; a separate currency badge and currency note are not shown. The form is not connected to storage.

### Transactions
Displays example expense history in a table. Search, category, month, and pagination controls are placeholders and do not filter records.

### Budgets
Displays an example monthly spending limit and category budget progress. The figures and progress bars do not update automatically.

### Savings
Displays three example savings goals and a form layout for a new goal. Submitting the form does not create or save a goal.

### Contact
Displays project contact information, a message form, and frequently asked questions. The contact form does not send messages.

## 3. Pakistan-oriented examples

The prototype uses amounts such as `Rs. 12,000`, dates in `DD-MM-YYYY` style, and examples such as Grocery/Rashan, electricity bills, petrol, JazzCash, and Easypaisa.

The visible `Rs.` prefix is intended to keep the interface concise. The application-wide currency code should be managed centrally as `PKR` when functional application logic is introduced.

## 4. Important usage note

SpendWise Phase 1 is a static demonstration. Do not enter real financial information or rely on the displayed values as a live record. Form submission, filtering, saving, and calculations are not implemented.

# SpendWise — Personal Expense Management Website

SpendWise is an academic Web Development project focused on helping individuals organize personal expenses, plan budgets, and track savings. The interface uses Pakistani financial conventions and a clean, responsive layout.

> **Current status:** Phase 1 — static HTML5 and CSS3 prototype. JavaScript, backend services, database storage, authentication, and persistent financial records are not implemented.

## Project objectives

- Present a clear overview of personal finances.
- Provide pages for recording and reviewing expenses.
- Demonstrate budget planning by category.
- Present savings goals and progress.
- Use a consistent, responsive interface across the website.
- Prepare a clear foundation for later functional development.

## Phase 1 features

The current prototype contains eight HTML pages:

| Page | File | Purpose |
|---|---|---|
| Home | `index.html` | Introduces SpendWise and highlights example financial figures. |
| About | `about.html` | Explains the project, its purpose, and objectives. |
| Dashboard | `dashboard.html` | Shows example balance, income, expenses, savings, and category summaries. |
| Add Expense | `add-expense.html` | Presents an expense-entry form with an `Amount` field and an `Rs.` prefix. |
| Expense History | `expense-history.html` | Displays sample expense records and visual filter controls. |
| Budget Planner | `budget-planner.html` | Shows a monthly budget and category-level progress. |
| Savings Goals | `savings-goals.html` | Displays example savings targets and a goal form. |
| Contact | `contact.html` | Presents project contact information, a message form, and FAQs. |

## Technology

- HTML5
- CSS3
- Visual Studio Code (recommended editor)
- Live Server extension (recommended local preview)

No JavaScript or backend technology is part of the current Phase 1 implementation.

## Project structure

```text
SpendWise/
├── index.html
├── about.html
├── dashboard.html
├── add-expense.html
├── expense-history.html
├── budget-planner.html
├── savings-goals.html
├── contact.html
├── css/
│   └── style.css
├── images/
└── docs/
    ├── PROJECT_OVERVIEW.md
    ├── USER_GUIDE.md
    ├── TECHNICAL_DOCUMENTATION.md
    ├── TESTING_CHECKLIST.md
    └── ROADMAP.md
```

The `images/` directory is reserved for project images. It may be empty if no local image assets are currently used.

## Run locally

### Option A — VS Code and Live Server

1. Open the `SpendWise` folder in Visual Studio Code.
2. Confirm that the eight HTML files and `css/style.css` are present.
3. Install the **Live Server** extension if it is not already installed.
4. Right-click `index.html`.
5. Select **Open with Live Server**.
6. Use the navigation links to visit the other pages.

### Option B — Browser

Open `index.html` directly in a modern browser. Live Server is recommended for a more convenient development workflow.

## Pakistan-specific conventions

The project is intended for use in Pakistan.

- **Internal currency code planned for the application:** `PKR`.
- **Visible amount format:** `Rs. 85,450`.
- Keep currency configuration centralized in the future application logic/backend. Do not store formatted strings such as `Rs. 85,450` as monetary values.
- Store monetary values as numeric/decimal amounts, with appropriate precision and validation.
- **Date display convention:** `DD-MM-YYYY`.
- Example local payment methods: Cash, JazzCash, Easypaisa, Bank Transfer, Debit Card, Credit Card.
- Example expense categories: Grocery/Rashan, Electricity, Gas, Water, Internet & Mobile, Petrol/Fuel, Transport, Education/Fees, Medical/Medicines, Rent, Shopping, Eating Out, and Other.

The current static HTML pages contain display examples only. Centralized currency handling is a future implementation requirement, not a completed backend feature.

## Important limitations

- Forms are visual HTML prototypes. They do not create or save records.
- Search and filter controls are not functional.
- Pagination controls are not connected to data.
- Budget totals and progress bars are static examples.
- Savings goals and progress are static examples.
- No login, user accounts, permissions, or authentication are implemented.
- No database, API, server-side validation, or persistent storage is implemented.
- The contact email shown in the prototype is a placeholder and must be replaced before any real deployment.
- Sample amounts and transactions are illustrative, not real financial data.

## Quality review items

Before presenting or extending the prototype, review:

1. Budget category allocations against the overall monthly budget. The six displayed category allocations currently total Rs. 44,000, while the overall budget is Rs. 50,000.
2. Expense History summary count versus the number of rows currently visible in the table. The page says 12 records but displays 7 rows.
3. Contact page placeholder email address.
4. Consistency of sample dates, month labels, and totals across all pages.
5. Navigation and responsive layout at desktop, tablet, and mobile widths.

## Documentation

- [Project Overview](docs/PROJECT_OVERVIEW.md)
- [User Guide](docs/USER_GUIDE.md)
- [Technical Documentation](docs/TECHNICAL_DOCUMENTATION.md)
- [Testing Checklist](docs/TESTING_CHECKLIST.md)
- [Development Roadmap](docs/ROADMAP.md)

## Academic project note

SpendWise is an academic prototype. Do not use its current sample figures as financial advice or as a live personal finance record. Complete security, privacy, validation, and data-integrity work before handling real user information.

# SpendWise — Technical Documentation

## 1. Current architecture

Phase 1 is a static, multi-page website:

- HTML files define page structure and content.
- `css/style.css` provides shared and page-specific presentation.
- Browser navigation loads each HTML page independently.
- There is no application server, API, JavaScript layer, or database in this phase.

## 2. Entry point

`index.html` is the website's home page and recommended starting point.

## 3. Page inventory

| File | Responsibility |
|---|---|
| `index.html` | Landing page |
| `about.html` | Project information |
| `dashboard.html` | Static financial overview |
| `add-expense.html` | Expense form presentation |
| `expense-history.html` | Static transaction table |
| `budget-planner.html` | Static budget overview |
| `savings-goals.html` | Static savings goals and form |
| `contact.html` | Contact information, form, and FAQs |
| `css/style.css` | Shared and page-specific styles |

## 4. Styling conventions

The established visual direction uses:

- Navy backgrounds and headings, including `#101E35`.
- Primary blue, including `#2563EB`.
- Light page backgrounds, including `#F8FAFC`.
- Green for positive or remaining-balance indicators.
- Arial as a common fallback font; use the project's existing font declarations as the source of truth.
- Shared navigation and footer patterns.
- CSS media queries for narrower viewports.

Avoid introducing a second, conflicting design system. When changing shared styles, check all eight pages.

## 5. Currency and financial data design

### Current prototype

The HTML contains static, preformatted examples such as `Rs. 85,450`. These are presentation strings, not values retrieved from a financial data model.

### Future implementation requirements

- Define the application currency centrally with ISO code `PKR`.
- Keep the visible amount format concise, such as `Rs. 85,450`.
- Do not store formatted values with the `Rs.` prefix in the database.
- Store monetary amounts using a suitable numeric/decimal representation.
- Apply one shared formatting function at the presentation boundary.
- Validate amount inputs and define rounding/precision rules.
- Ensure totals are calculated from numeric values, not by parsing display strings.
- Use `DD-MM-YYYY` for the agreed user-facing date convention while storing dates in an unambiguous machine-readable format.

These are design requirements for future phases; they are not implemented by the current HTML/CSS prototype.

## 6. Suggested future data entities

Potential entities for a later backend include:

- User: account identity and authentication metadata.
- Expense: amount, date, category, payment method, description, and owner.
- Income: amount, date, source, and owner.
- Budget: period, category, and allocated amount.
- SavingsGoal: title, target amount, saved amount, target date, and status.

These are proposed domain concepts only. No database schema currently exists.

## 7. Security and privacy requirements for later phases

Before handling real financial information:

- Use secure authentication and authorization.
- Enforce server-side validation.
- Restrict users to their own records.
- Protect secrets and credentials outside source control.
- Use HTTPS in deployed environments.
- Avoid logging sensitive financial information.
- Define backup, retention, and deletion policies.
- Test access control and common web vulnerabilities.

## 8. Maintenance

- Keep shared navigation labels and links consistent across pages.
- Keep common styling in `css/style.css`.
- Use semantic HTML elements and descriptive labels.
- Test all pages after modifying shared CSS.
- Keep documentation updated when scope or implementation changes.

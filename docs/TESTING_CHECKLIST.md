# SpendWise — Phase 1 Testing Checklist

Use this checklist during manual review. Mark an item complete only after checking it in the browser.

## A. Project setup

- [ ] Project opens in Visual Studio Code.
- [ ] `index.html` opens in a browser.
- [ ] `css/style.css` loads on every page.
- [ ] No missing local assets are reported by the browser.

## B. Page availability

- [ ] `index.html`
- [ ] `about.html`
- [ ] `dashboard.html`
- [ ] `add-expense.html`
- [ ] `expense-history.html`
- [ ] `budget-planner.html`
- [ ] `savings-goals.html`
- [ ] `contact.html`

## C. Navigation

- [ ] Logo links to Home.
- [ ] Every navigation link opens the correct page.
- [ ] Add Expense links open `add-expense.html`.
- [ ] Active navigation styling matches the current page.
- [ ] Footer links and page transitions do not lead to missing files.

## D. Visual consistency

- [ ] Header and navigation are consistent across pages.
- [ ] Footer styling is consistent across pages.
- [ ] Typography and heading hierarchy are consistent.
- [ ] Navy, blue, and light background colours are used consistently.
- [ ] Cards, forms, tables, and buttons have consistent spacing.
- [ ] No horizontal overflow occurs at common viewport widths, except intentional table scrolling.

## E. Responsive layout

- [ ] Home page at desktop width.
- [ ] Dashboard at desktop width.
- [ ] Expense history table can be inspected on a narrow screen.
- [ ] Budget cards wrap appropriately.
- [ ] Savings cards and form stack appropriately.
- [ ] Contact form stacks on a narrow screen.
- [ ] Navigation remains usable on mobile. If it does not, record it as a defect for correction.

## F. Forms and controls

- [ ] Required fields show native browser validation where configured.
- [ ] Email field uses the email input type.
- [ ] Numeric amount fields have sensible minimum values where configured.
- [ ] Add Expense labels the amount field `Amount *` and displays `Rs.` as its input prefix without a separate currency badge or note.
- [ ] Reset controls reset their respective forms.
- [ ] Static forms are clearly understood not to save or send data.
- [ ] Search, filter, and pagination controls are recognized as non-functional placeholders.

## G. Data and content consistency

- [ ] Monetary values use the visible `Rs.` convention.
- [ ] Currency is not repeatedly explained in page content.
- [ ] Dates follow `DD-MM-YYYY` in displayed sample records.
- [ ] Category names are consistent across pages.
- [ ] Payment methods use the agreed Pakistan-oriented examples.
- [ ] Dashboard arithmetic is correct.
- [ ] Budget category allocations reconcile with the overall budget.
- [ ] Transaction record count matches the number of records actually shown.
- [ ] Placeholder contact details are identified and replaced before any public release.

## H. Phase 1 scope verification

- [ ] No JavaScript has been added as part of Phase 1.
- [ ] No backend or database is claimed to exist.
- [ ] No form is represented as persisting data.
- [ ] Documentation accurately describes the prototype as static HTML/CSS.

## Known review items

- The Budget Planner's six displayed category allocations total Rs. 44,000, while the overall budget is Rs. 50,000. Reconcile the difference or explain the unallocated amount.
- Expense History indicates 12 records but the current markup displays 7 rows. Add the missing rows or change the summary.
- The contact email `support@spendwise.example` is a placeholder, not a verified support address.

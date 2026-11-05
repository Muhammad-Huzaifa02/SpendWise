# SpendWise — Development Roadmap

## Current status

**Phase 1: Static UI prototype (HTML5 + CSS3)**

The project has eight HTML pages and a shared stylesheet. The forms, filters, tables, progress bars, and financial figures are static examples. No JavaScript, backend, database, authentication, or persistence is currently implemented.

## Phase 1 — Review and stabilization

Before adding functionality:

1. Review all eight pages in the browser.
2. Fix broken navigation and missing assets.
3. Standardize shared header, footer, typography, spacing, and responsive behavior.
4. Reconcile all sample totals and record counts.
5. Replace placeholder contact details if real contact details are approved.
6. Confirm the page structure and requirements with the project supervisor/team.

**Exit criteria:** all pages are navigable, visually consistent, responsive, and internally consistent.

## Phase 2 — JavaScript interactions

Planned work:

- Add client-side form handling and validation.
- Implement expense list rendering from structured data.
- Implement search and category/month filtering.
- Implement pagination.
- Calculate income, expenses, balance, and category totals.
- Calculate budget usage and remaining amounts.
- Calculate savings-goal progress.
- Add clear empty states and error messages.

A temporary browser storage layer may be used only if it is appropriate for the course requirements. It must not be presented as a secure multi-user financial database.

**Exit criteria:** interactions work with test data and calculations pass defined test cases.

## Phase 3 — Backend and database

Choose the backend stack based on course requirements and team capability. Design APIs and a database for users, expenses, income, budgets, and savings goals.

Planned work:

- Define the data model and relationships.
- Implement API endpoints.
- Add server-side validation.
- Persist records in a database.
- Add centralized `PKR` currency configuration.
- Store numeric monetary values rather than formatted display strings.
- Implement consistent date and amount handling.

**Exit criteria:** application data persists and can be retrieved reliably through the backend.

## Phase 4 — Authentication and user security

Planned work:

- Registration and login.
- Secure password handling.
- Session/token management.
- Authorization and per-user data isolation.
- Password reset flow, if required.
- Security and privacy review.

**Exit criteria:** users can access only the records they are authorized to view or change.

## Phase 5 — Reporting and usability improvements

Potential enhancements:

- Monthly and yearly reports.
- Expense category comparisons.
- Export to CSV or PDF.
- Budget alerts.
- Improved accessibility.
- More complete mobile experience.

Prioritize features according to project requirements and available time.

## Phase 6 — Quality assurance and deployment

Planned work:

- Functional and integration testing.
- Security testing.
- Cross-browser and responsive testing.
- Data integrity and edge-case testing.
- Deployment configuration.
- Backup and recovery planning.
- Final user documentation.

**Exit criteria:** the release is tested, documented, and deployed in an environment appropriate for the project.

## Pakistan-specific requirements across future phases

- Use `PKR` as the internal currency code.
- Display amounts using the concise `Rs.` prefix and consistent digit grouping.
- Keep currency formatting centralized rather than duplicating rules across pages.
- Store numeric amounts, not formatted currency strings.
- Use `DD-MM-YYYY` as the agreed display date format.
- Support relevant local payment method labels such as Cash, JazzCash, Easypaisa, Bank Transfer, Debit Card, and Credit Card.
- Include locally relevant categories such as Rashan, electricity, gas, petrol, education, and medical expenses.

## Scope control

Do not start Phase 2 until the Phase 1 review is complete. Treat every item above as planned work unless it is visibly implemented and tested in the project.

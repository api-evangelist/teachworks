# Teachworks (teachworks)

Teachworks is business management software for tutoring companies, music schools, test-prep centers, and other education businesses. It handles scheduling, student and family CRM, teacher management, lesson and event calendars, online billing and invoicing, payments, and teacher wages. The Teachworks API is a REST API (base `https://api.teachworks.com/v1`, token authentication over HTTPS) that exposes account data - customers, students, employees, lessons, services, invoices, payments, and wages - so companies can build custom integrations. The API is available on the Growth and Premium plans. There is no native webhook or WebSocket surface; event-driven integrations are delivered through Zapier, Make, and Integrately polling.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/teachworks/refs/heads/main/apis.yml)

## Authentication

Requests are authenticated with an account API token passed in the `Authorization` header using the scheme `Authorization: Token token=API_TOKEN`. Generate a token on the Integrations and Add-ons page in Teachworks. All requests must be made over HTTPS. List endpoints paginate 20 records per page (up to 80 via `per_page`), and the API is rate limited to 4 requests per second per token.

## Tags

- Education
- Tutoring
- EdTech
- Scheduling
- Business Management
- CRM
- Billing

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Teachworks Customers API

List, retrieve, create, and update customer profiles - the billing account that is either a family or an independent student. Create families and independent students, set custom field values, and retrieve lesson totals for a customer.

- **Human URL:** [https://documenter.getpostman.com/view/10096149/SWTABydD](https://documenter.getpostman.com/view/10096149/SWTABydD)
- **Base URL:** `https://api.teachworks.com/v1`

### Teachworks Students API

List, retrieve, create, and update students - both child students belonging to a family and independent students. Set custom field values and retrieve per-student lesson totals.

- **Human URL:** [https://documenter.getpostman.com/view/10096149/SWTABydD](https://documenter.getpostman.com/view/10096149/SWTABydD)
- **Base URL:** `https://api.teachworks.com/v1`

### Teachworks Employees API

Manage employees (teachers and staff) - list, retrieve, create, and update employees, set their status, set custom field values, and retrieve an employee's earnings and lesson totals.

- **Human URL:** [https://documenter.getpostman.com/view/10096149/SWTABydD](https://documenter.getpostman.com/view/10096149/SWTABydD)
- **Base URL:** `https://api.teachworks.com/v1`

### Teachworks Lessons API

List, retrieve, and create lessons; add students to a lesson and mark a lesson complete. Lesson participants expose the per-student rows attached to each lesson.

- **Human URL:** [https://documenter.getpostman.com/view/10096149/SWTABydD](https://documenter.getpostman.com/view/10096149/SWTABydD)
- **Base URL:** `https://api.teachworks.com/v1`

### Teachworks Events and Availability API

List and retrieve non-teaching calendar events (other events) and read employee availabilities and unavailabilities that drive scheduling.

- **Human URL:** [https://documenter.getpostman.com/view/10096149/SWTABydD](https://documenter.getpostman.com/view/10096149/SWTABydD)
- **Base URL:** `https://api.teachworks.com/v1`

### Teachworks Services and Subjects API

Read the catalog that lessons are built from - services, subjects, student groups, wage tiers, and cost premiums - plus create, retrieve, and update locations where lessons are delivered.

- **Human URL:** [https://documenter.getpostman.com/view/10096149/SWTABydD](https://documenter.getpostman.com/view/10096149/SWTABydD)
- **Base URL:** `https://api.teachworks.com/v1`

### Teachworks Invoices API

List and retrieve customer invoices and read credit note allocations that apply credits against invoices.

- **Human URL:** [https://documenter.getpostman.com/view/10096149/SWTABydD](https://documenter.getpostman.com/view/10096149/SWTABydD)
- **Base URL:** `https://api.teachworks.com/v1`

### Teachworks Payments API

List, retrieve, create, and update customer payments, and list, retrieve, and create payment allocations that apply a payment to specific invoices.

- **Human URL:** [https://documenter.getpostman.com/view/10096149/SWTABydD](https://documenter.getpostman.com/view/10096149/SWTABydD)
- **Base URL:** `https://api.teachworks.com/v1`

### Teachworks Wages API

Manage teacher pay - list, retrieve, create, and update wage payments, and list, retrieve, and create other compensation records outside of lesson wages.

- **Human URL:** [https://documenter.getpostman.com/view/10096149/SWTABydD](https://documenter.getpostman.com/view/10096149/SWTABydD)
- **Base URL:** `https://api.teachworks.com/v1`

### Teachworks Results and Repertoires API

Track student progress - list, retrieve, create, and update results and result groups, and manage repertoire items (for music lessons) attached to students.

- **Human URL:** [https://documenter.getpostman.com/view/10096149/SWTABydD](https://documenter.getpostman.com/view/10096149/SWTABydD)
- **Base URL:** `https://api.teachworks.com/v1`

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/teachworks)
- [Website](https://teachworks.com)
- [Documentation](https://teachworks.com/addons/api)
- [Plans](plans/teachworks-plans-pricing.yml)
- [Rate Limits](rate-limits/teachworks-rate-limits.yml)
- [Fin Ops](finops/teachworks-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

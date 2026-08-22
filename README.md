# Teachworks (teachworks)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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

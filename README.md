# LEAP (leap-legal)

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

LEAP is cloud-based legal practice management software for law firms, covering matter and contact management, document automation and court forms, time recording, billing, and trust accounting, tightly integrated with Microsoft 365. LEAP operates a LEAP Developer Console and LEAP Marketplace (developer.leap.build / console.leap.build) through which approved third-party developers build REST-based integrations (an "API Reference" is versioned there, e.g. v1.0.4, v1.0.5), but the technical reference - endpoint paths, base URL, and authentication schema - sits behind developer registration and an app review process rather than a public, self-serve API reference. There is no publicly published OpenAPI document, public base URL, or anonymous API key signup. Existing Marketplace integrations (Xero, Zoom, InfoTrack, LawTap, and others) confirm the API surface is real and in production use, but its concrete shape is not publicly disclosed.

**Access model:** Gated / partner-provisioned. Free developer registration at console.leap.build, followed by building against a login-gated API reference, then app submission and review before Marketplace listing. No public OpenAPI document, no anonymous API key signup. See [review.yml](review.yml) for the full findings.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/leap-legal/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/leap-legal/refs/heads/main/apis.yml)

## Tags

- Legal
- LegalTech
- Practice Management
- Legal Accounting
- Trust Accounting
- Document Automation

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs

*All APIs below are modeled capability groupings (`endpointsModeled: true`) inferred from LEAP's marketed product features, its developer knowledge base, and confirmed live Marketplace integrations - not from a crawled technical reference, since LEAP's API Reference is gated behind developer console login.*

### LEAP Matters & Contacts API

Modeled matter and contact/client management surface that third-party Marketplace apps integrate against - matters (number, title, practice area, status, responsible attorney), contacts/clients (individuals, organizations), and party roles. Confirmed to exist by LEAP's Marketplace apps and the "Configure LEAP Data" developer questionnaire, but no endpoint paths, base URL, or schema are publicly published.

- **Human URL:** [https://developer.leap.build/knowledge-base/general/general-getting-started/](https://developer.leap.build/knowledge-base/general/general-getting-started/)

#### Tags

- Matters
- Clients
- Contacts
- Conflict Checks

#### Properties

- [Documentation](https://developer.leap.build/knowledge-base/general/general-getting-started/)
- [Documentation](https://developer.leap.build/knowledge-base/general/configure-leap-data/)

### LEAP Time & Billing API

Modeled time recording, invoicing, and billing surface, evidenced by LEAP's own marketed "automatic timekeeping" and "multiple billing and payment options" features and by production Marketplace integrations such as Xero for accounting sync. No public endpoint list, base URL, or request/response schema is disclosed.

- **Human URL:** [https://www.leap.build/](https://www.leap.build/)

#### Tags

- Time Recording
- Invoicing
- Billing

#### Properties

- [Documentation](https://www.leaplegalsoftware.com/us/integrations/)

### LEAP Trust Accounting API

Modeled trust ledger surface (receipts, disbursements, transfers, balances) reflecting LEAP's marketed legal/trust accounting functionality, a core, heavily regulated feature of the practice management product. No public endpoint list, base URL, or schema is disclosed for programmatic trust-accounting access.

- **Human URL:** [https://www.leap.com.au/features/legal-content/](https://www.leap.com.au/features/legal-content/)

#### Tags

- Trust Accounting
- Legal Accounting
- Compliance

#### Properties

- [Documentation](https://www.leaplegalsoftware.com/us/pricing/)

### LEAP Documents API

Modeled document metadata and automation surface - LEAP's core "automated legal documents" and court-form assembly capability, tightly coupled to Microsoft 365. Marketplace developers demonstrate document/integration behavior as part of the app review process, but no public endpoint list, base URL, or schema is disclosed.

- **Human URL:** [https://developer.leap.build/knowledge-base/general/demonstrating-your-integration-with-leap/](https://developer.leap.build/knowledge-base/general/demonstrating-your-integration-with-leap/)

#### Tags

- Documents
- Document Automation
- Court Forms

#### Properties

- [Documentation](https://developer.leap.build/knowledge-base/general/demonstrating-your-integration-with-leap/)
- [Documentation](https://developer.leap.build/knowledge-base/general/general-submission-process/)

### LEAP Calendar API

Modeled calendar/diary and appointment-scheduling surface, evidenced by production Marketplace scheduling integrations (e.g. LawTap) and Microsoft 365 calendar integration. No public endpoint list, base URL, or schema is disclosed.

- **Human URL:** [https://marketplace.leap.build/en-AU/apps](https://marketplace.leap.build/en-AU/apps)

#### Tags

- Calendar
- Scheduling
- Diary

#### Properties

- [Documentation](https://marketplace.leap.build/en-AU/apps)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/leap-legal-software-usa)
- [Website](https://leap.us)
- [Documentation](https://developer.leap.build/)
- [Plans](plans/leap-legal-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

# LEAP (leap-legal)

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

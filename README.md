# HigherGov MCP

The HigherGov MCP connects AI assistants and LLM tools to HigherGov’s market-leading federal, state, local, and proprietary government data.

MCP stands for **Model Context Protocol**. It is a standard way for AI assistants to securely connect to external tools and data sources. With the HigherGov MCP, supported AI assistants can search and analyze opportunities, awards, contractors, documents, NSNs, DIBBS-related records, and related government market intelligence using natural language.

The HigherGov MCP is powered by the HigherGov API and is available to HigherGov subscribers.

> This feature is currently in beta. If you have use cases not currently supported, please send suggestions to [contact@highergov.com](mailto:contact@highergov.com).

---

## MCP Endpoint

```text
https://www.highergov.com/mcp/
```

## Create an API Key

To use the HigherGov MCP, you need a HigherGov API key.

You can create and manage API keys here:

```text
https://www.highergov.com/api-management/

---

## What You Can Do

Use HigherGov MCP to ask questions such as:

```text
Find active federal contract opportunities for cybersecurity services.
```

```text
Find low-competition federal and SLED IT opportunities in Virginia and recommend teaming partners.
```

```text
Search recent federal contract awards for zero trust.
```

```text
Find potential small business partners with federal health agency experience.
```

```text
Review the solicitation documents and identify submission requirements.
```

```text
Find active SLED opportunities for construction services in Texas.
```

```text
Research the incumbent contractor for this recompete opportunity.
```

```text
Find companies with relevant prior performance for this opportunity.
```

---

## Data Coverage

HigherGov MCP provides access to HigherGov’s comprehensive government market data, including federal, state, local, and proprietary datasets.

Sources and data coverage include:

| Source / Dataset | Coverage |
|---|---|
| **SAM.gov** | Federal contract opportunities, notices, solicitations, awards-related opportunity data, and federal procurement records. |
| **Grants.gov** | Federal grant opportunities and related grant notices. |
| **SLED Opportunities** | State, local, and education opportunities from thousands of agencies and public entities. |
| **USAspending** | Federal spending, contracts, grants, loans, direct payments, and assistance data. |
| **FPDS** | Federal Procurement Data System contract award and transaction data. |
| **DIBBS** | Defense Logistics Agency procurement opportunities and related DIBBS data. |
| **NSN Data** | NATO Stock Number data, supplier references, part-number research, and related defense supply chain information. |
| **Federal Contract Awards** | Historical federal contract awards, modifications, obligations, agencies, vendors, NAICS, PSCs, and contract vehicles. |
| **Federal IDVs / Vehicles** | IDIQs, GWACs, BPAs, BOAs, and other federal contract vehicles. |
| **Federal Grants** | Federal grant awards by agency, program, recipient, geography, and topic. |
| **Federal Subcontracts** | Federal subcontract activity, prime/sub relationships, and subcontract award history. |
| **Federal Subgrants** | Subgrant activity, recipient relationships, and grant funding flows. |
| **Contractor / Awardee Profiles** | Company profiles, UEI, CAGE, NAICS, PSC, registrations, capabilities, agency experience, vehicles, and award history. |
| **Opportunity Documents** | Solicitation documents, attachments, extracted text, requirements, due dates, instructions, evaluation criteria, and proposal-relevant content. |
| **HigherGov Proprietary Data** | HigherGov-enriched opportunity, award, contractor, market, and competition intelligence. |
| **60K+ Other Sources** | Additional government, agency, procurement, market, contractor, and public-sector data sources used across HigherGov. |

---

## Available MCP Tools

The HigherGov MCP exposes tools that allow AI assistants to search HigherGov data and retrieve supporting records.

In most cases, you do **not** need to know the tool names. You can ask questions naturally, and your AI assistant will select the appropriate tool.

| Category | Tool | Description | Example Uses |
|---|---|---|---|
| Opportunity Search | `search_opportunities` | Search federal, state, local, forecast, grant, DIBBS, and related opportunities. | Find active opportunities, identify opportunities by NAICS/customer/topic, search federal and SLED opportunities together, monitor saved searches, find low-competition opportunities. |
| Opportunity Documents | `get_opportunity_documents` | Retrieve documents and extracted text for an opportunity. | Summarize solicitations, extract requirements, review due dates, identify submission instructions, analyze evaluation criteria, support proposal writing. |
| Federal Contract Awards | `search_federal_contracts` | Search historical federal contract awards. | Research prior awards, identify incumbents, analyze buying patterns, find awards by agency, NAICS, PSC, company, or topic. |
| Federal IDVs | `search_federal_idvs` | Search federal IDVs, GWACs, BPAs, BOAs, IDIQs, and other contract vehicles. | Research contract vehicles, identify vehicle holders, understand vehicle usage, find recompete or partner opportunities. |
| Federal Grants | `search_federal_grants` | Search federal grant awards. | Research grant awards by topic, recipient, program, agency, or geography. |
| Federal Subcontracts | `search_federal_subcontracts` | Search federal subcontract activity. | Identify subcontract relationships, find primes or subs, research company participation, analyze teaming networks. |
| Federal Subgrants | `search_federal_subgrants` | Search federal subgrant activity. | Research subgrant recipients, funding flows, grant ecosystems, and related organizations. |
| Contractor and Partner Search | `search_awardees` | Search companies, contractors, awardees, and potential teaming partners. | Find partners by capability, NAICS, UEI, CAGE, agency experience, vehicles, business type, location, certifications, or prior performance. |
| Contractor Detail | `get_awardee_detail` | Retrieve detailed company or awardee profiles. | Review registrations, NAICS codes, PSC codes, business types, capabilities, agency experience, vehicles, and related award history. |
| NSN / DIBBS Research | `search_nsn` | Search NATO Stock Number and DIBBS-related data. | Look up NSNs, search by part number, find suppliers by CAGE code, review supplier and award history. |

---

## Common Use Cases

### Find and Analyze Opportunities

Search federal, state, local, forecast, grant, and DIBBS opportunities, then analyze fit, timing, value, requirements, and competitive posture.

Example prompts:

```text
Find active federal contract opportunities for custodial services.
```

```text
Search active federal and state/local opportunities for physical security or surveillance.
```

```text
Find active federal opportunities under NAICS 541512 related to zero trust.
```

```text
Search federal forecasts related to IT modernization.
```

```text
Find upcoming SLED forecast opportunities for construction services.
```

```text
Find low-competition federal and SLED IT opportunities in Virginia.
```

```text
Find opportunities that match our cybersecurity capabilities and prioritize them by fit.
```

---

### Review Documents and Support Proposal Work

Retrieve opportunity documents and extracted text to summarize requirements, instructions, dates, evaluation criteria, and scope. Use document-level analysis to support capture and proposal workflows.

Example prompts:

```text
Find active opportunities for janitorial services and summarize the documents for the top result.
```

```text
Get the documents for this opportunity and summarize the scope of work.
```

```text
Review the solicitation documents and identify submission requirements.
```

```text
Extract the evaluation criteria and turn them into a proposal compliance checklist.
```

```text
Summarize the required forms, attachments, and due dates for this solicitation.
```

```text
Draft a proposal outline based on the solicitation requirements.
```

---

### Research Awards

Analyze historical contracts, grants, vehicles, spending, incumbents, likely recompetes, and agency buying behavior.

Example prompts:

```text
Search federal contract awards for zero trust under NAICS 541512.
```

```text
Find federal contracts awarded to this UEI.
```

```text
Search IDVs involving cloud migration.
```

```text
Search federal grant awards related to workforce development.
```

```text
Find subcontract awards involving this company.
```

```text
Who are the incumbent contractors for this agency and requirement area?
```

```text
Analyze spending trends for cybersecurity services at this agency over the last five years.
```

---

### Find Contractors and Teaming Partners

Search for companies by capability, location, NAICS, PSC, UEI, CAGE, agency experience, certifications, vehicles, and prior performance.

Example prompts:

```text
Find potential teaming partners for cybersecurity work.
```

```text
Find small business partners with experience in physical security.
```

```text
Find the UEI and CAGE code for Leidos.
```

```text
Get the detailed profile for this UEI.
```

```text
Find companies with primary NAICS 541611 and federal health agency experience.
```

```text
Find Virginia-based IT contractors with prior SLED wireless networking experience.
```

```text
Find potential partners with relevant prior performance for this opportunity.
```

---

### Research NSNs and DIBBS-Related Data

Search NATO Stock Numbers, part numbers, suppliers, and related award history.

Example prompts:

```text
Look up NSN 6505013306269.
```

```text
Find NSNs associated with CAGE 95403.
```

```text
Search for this part number and summarize suppliers.
```

```text
Find recent supplier and award history for this NSN.
```

---

## Authentication

The preferred authentication method is to send your HigherGov API key as a bearer token:

```http
Authorization: Bearer YOUR_HIGHERGOV_API_KEY
```

Some MCP clients support custom headers directly. If your client does, use the bearer-token method above.

Some AI assistants or MCP clients may refer to this value as an **Access Token**, **API Key**, or **Authorization Header**.

---

## Creating a HigherGov API Key

API keys can be managed from the HigherGov API Management screen. Admin access may be required.

General steps:

1. Sign in to HigherGov.
2. Select the gear icon in the upper-right corner.
3. Select **API**.
4. Click **Generate Key**.
5. Copy and securely save the key.

> Important: the full API key is only displayed once when it is created. Make sure to copy and securely store it before leaving the page.

---

## Connecting to HigherGov MCP

MCP support is changing quickly across AI providers. Exact setup steps may vary by client, plan, and workspace configuration.

At a high level:

1. Open your AI assistant’s MCP, Connector, App, or Tools settings.
2. Add a new remote MCP server.
3. Enter the HigherGov MCP endpoint:

```text
https://www.highergov.com/mcp/
```

4. Configure authentication:

```http
Authorization: Bearer YOUR_HIGHERGOV_API_KEY
```

5. Save or scan tools.
6. Start asking questions naturally.

---

## Claude

Claude supports custom connectors using remote MCP servers.

Use:

```text
https://www.highergov.com/mcp/
```

Authentication:

```http
Authorization: Bearer YOUR_HIGHERGOV_API_KEY
```

General steps:

1. Open Claude.
2. Go to **Settings → Connectors**.
3. Select **Add custom connector**.
4. Enter the HigherGov MCP URL.
5. Add authentication if supported by your Claude plan or client.
6. Enable the connector in a chat.
7. Ask questions naturally.

Example prompts:

```text
Find active federal contract opportunities for cybersecurity services.
```

```text
Find potential teaming partners for cybersecurity work.
```

```text
Search recent federal contract awards for zero trust.
```

---

## OpenAI / ChatGPT

OpenAI supports remote MCP servers through ChatGPT apps/connectors and through the OpenAI API. Availability may depend on your workspace and plan.

Use:

```text
https://www.highergov.com/mcp/
```

Authentication:

```http
Authorization: Bearer YOUR_HIGHERGOV_API_KEY
```

General steps:

1. Confirm your workspace supports custom MCP apps/connectors.
2. Enable Developer Mode if required.
3. Create a new custom app or connector.
4. Provide the HigherGov MCP endpoint.
5. Configure authentication using your HigherGov API key.
6. Scan tools.
7. Test the app in a new chat.
8. Publish or enable it for your workspace if desired.

Example API configuration shape:

```json
{
  "tools": [
    {
      "type": "mcp",
      "server_label": "highergov",
      "server_url": "https://www.highergov.com/mcp/",
      "authorization": "Bearer YOUR_HIGHERGOV_API_KEY"
    }
  ]
}
```

---

## Gemini CLI

Gemini CLI supports MCP servers through `settings.json` or the `gemini mcp add` command.

Use:

```text
https://www.highergov.com/mcp/
```

Add with CLI command:

```bash
gemini mcp add \
  --transport http \
  --header "Authorization: Bearer YOUR_HIGHERGOV_API_KEY" \
  highergov \
  https://www.highergov.com/mcp/
```

Verify the connection:

```bash
gemini mcp list
```

Or configure `settings.json`:

```json
{
  "mcpServers": {
    "highergov": {
      "httpUrl": "https://www.highergov.com/mcp/",
      "headers": {
        "Authorization": "Bearer YOUR_HIGHERGOV_API_KEY"
      },
      "timeout": 30000
    }
  }
}
```

---

## Example Workflow

Prompt:

```text
Find low-competition federal and SLED IT opportunities in Virginia and recommend teaming partners.
```

Example response:

```text
I found several active Virginia IT opportunities where competition may be lower based on HigherGov analysis.

Opportunity:
Quick Quote – Wi‑Fi Survey & Wireless Assessment Services

Market:
SLED

Location / Agency:
Richmond, VA – Capital Region Airport Commission

Due:
2026-09-07

Estimated Value:
$75K–$225K

Competition:
Competition may be lower due to specialized airport, secure-facility, and high-density wireless survey requirements.

Recommended Posture:
Prime if you have Wi‑Fi survey tools and airport references; otherwise team with a local network integrator.

Potential Teaming Partner:
Company A – Virginia Network Integrator

Why:
Strong potential fit based on local presence, relevant NAICS alignment, prior public-sector network projects, and secure-facility experience.

Additional Partner:
Company B – Airport IT Services Contractor

Why:
Useful partner if the bid requires airport references, onsite coordination, or prior performance in transportation environments.
```

---

## Example Prompts by Workflow

### Opportunity Search

```text
Find active federal contract opportunities for janitorial services.
```

```text
Search active federal and state/local opportunities for physical security or surveillance.
```

```text
Find active federal opportunities under NAICS 541512 related to zero trust.
```

```text
Search federal forecasts related to IT modernization.
```

```text
Find upcoming SLED forecast opportunities for construction services.
```

---

### Opportunity Documents

```text
Find active opportunities for janitorial services and summarize the documents for the top result.
```

```text
Get the documents for this opportunity and summarize the scope of work.
```

```text
Review the solicitation documents and identify submission requirements.
```

```text
Create a compliance matrix from the solicitation documents.
```

```text
Summarize the evaluation criteria and proposal instructions.
```

---

### Award Research

```text
Search federal contract awards for zero trust under NAICS 541512.
```

```text
Find federal contracts awarded to this UEI.
```

```text
Search IDVs involving cloud migration.
```

```text
Search federal grant awards related to workforce development.
```

```text
Find subcontract awards involving this company.
```

---

### Contractor and Partner Research

```text
Find potential teaming partners for cybersecurity work.
```

```text
Find small business partners with experience in physical security.
```

```text
Find the UEI and CAGE code for Leidos.
```

```text
Get the detailed profile for this UEI.
```

```text
Find companies with primary NAICS 541611 and federal health agency experience.
```

---

### NSN / DIBBS Research

```text
Look up NSN 6505013306269.
```

```text
Find NSNs associated with CAGE 95403.
```

```text
Search for this part number and summarize suppliers.
```

---

## Notes

- HigherGov MCP is available to HigherGov subscribers.
- Each subscription includes API/MCP usage subject to the terms of the subscriber’s plan.
- Supported clients and MCP configuration steps may change as AI assistants update their MCP and connector support.
- You generally do not need to call individual tools by name. Ask natural-language questions and your AI assistant will choose the appropriate HigherGov MCP tools.

---

## Support

For access, setup questions, or feature suggestions, contact:

```text
contact@highergov.com
```

Documentation:

```text
https://docs.highergov.com/import-and-export/highergov-mcp
```

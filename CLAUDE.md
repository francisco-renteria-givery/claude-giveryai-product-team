# Givery AI Team – Notion workspace project

This project (and every session in it) works on the Givery AI Team Notion page.

- **Root page:** Givery AI Team
- **URL:** https://app.notion.com/p/givery/Givery-AI-Team-4076931cc44980768eb5cbaab4241568
- **Page ID:** `4076931cc44980768eb5cbaab4241568`
- Use the Notion MCP tools (`notion-fetch`, `notion-update-page`, `notion-create-pages`, `notion-create-database`) against this page ID.
- Goal: a team hub with members, news, team rules, and general information.

## Page structure
```
Givery AI Team (root)
├── Sections (inline gallery "Cards") – data source `collection://e84d34fd-76a4-4504-ae76-8f21d9e3cff1` (Name, Tagline, Order)
│   ├── Team      `4076931cc44981818098cd10351e5de6` – linked view of Members
│   ├── News      `4076931cc44981c69b97e12caf17354e` – linked view of News
│   ├── Meetings  `4076931cc449818284e7c580a21f3cd1` – linked view of Meetings
│   ├── About `4076931cc449812eb6b0d2fec60e6360`
│   ├── Rules `4076931cc4498105b618cd545fe311a2`
│   └── Onboarding `4076931cc4498141ae87c958d65632c4` – includes linked Slack Channels table
└── Databases `4076931cc44981b59b3df770c3db9d65` – all source databases live here
    ├── Members – `collection://1aff5912-2f89-477d-802d-f58f8a551cb9`
    ├── News & Announcements – `collection://660f9819-3952-4879-9cdf-41bed05ac8d9`
    ├── Meetings & Rituals – `collection://64078b8f-b1d3-486f-b0fb-bf44260d2119`
    └── Slack Channels – `collection://3bfdf717-8b64-47f1-b95f-6cbd1ed35fc5` (giveryai_prod_*; "prod" = Product)
```
Hub Communication section = short static summary of channels; full table lives in Onboarding.
Rule: new databases go in **Databases**; the hub and section pages show only linked views.
Style: Givery brand (red #C80000 / black / white): red_bg banner callouts, red ● before headings, logo cover.

## Projects: link, never duplicate
The team has 2 projects, each with its own Notion page. The hub only links to them:
- 法務dx (Legal DX, TENA) – `4066931cc44980f8bddde488bc32ba2b`
- Givery AI Recorder – `3f36931cc44980ebb34fc1cdddb83673`
- Note: "Givery AI Home" (`36a6931cc449806dbbbae905a627aab2`) is NOT a project.

## Project governance
Each project has a Governance page (roles, decision rights, release gates, escalation, safeguards) under its Product Development page, with its own Decision Register database. Governance lives in the project, not the hub.
- **Givery AI Recorder** – Product Development `3f36931cc449814f80efd8876f101800`
  - Governance `4076931cc44981cfb9a6e67a1c4145c5`
  - Decision Register – `collection://884a62c1-9519-4d33-8829-4626bf3df8b2` (IDs `REC-DEC-n`; relation to Recorder Releases)
  - Roles: Product Head = Francisco; Business Owner = Tsuboi-san (坪井琢磨, no deputy); Project Manager = Miri; Product Manager and Engineering Lead vacant (covered by Francisco); QA = Pinta (can block releases).
  - Release gates tiered by channel (firmware / mobile app / portal+backend).
- **法務dx (TENA)** – Product Development `4086931cc44981878b1ee895fe662e77`
  - Governance `4086931cc44981caa88fc9998997190b`
  - Decision Register – `collection://a8df0c6c-48f5-424d-8213-bedcebcb4d1c` (IDs `TENA-DEC-n`); backfilled with 23 Historical entries from the Handover page (Reconstructed/Unconfirmed, no decision owners).
  - All roles are ⟨TBD⟩ placeholders; development paused from November 2026.
  - Incidents – `collection://76f24548-078d-4316-95a8-e83af3d119a4` (IDs `TENA-INC-n`); while paused only Critical (login down, data loss/corruption, security incident) is handled now, the rest is "Log for restart".
  - Main page layout (mirrors Recorder): header callout, environments, tools, 4 columns → Product Overview `4086931cc44981d1b34cfe4eeb05f600`, Roadmap `4086931cc44981d6b467ee688fc419a6`, Product Development, Resources `4086931cc4498100965cd9e2d9182eab` (holds the Handover page and "Handover meeting – 2026-10-27"); then Support while paused, Open items, linked views of Incidents and Decision Register.
  - Legal contact: Kondo-san (近藤永生). Never put login credentials on the main page.
- Safeguards (both projects): QA overrides, skipped/waived gates and hotfixes always need a Decision Register entry; any interim role concentration is shown as "Vacant — covered by …".
- Historical entries: mark Verified / Reconstructed / Unconfirmed; never attribute decision owners without evidence.
- Team-facing pages must not reference individual feedback that led to the governance work.

## Team members (6)
The Members database holds roles, basic info (Name (JP), Joined Givery, Skills) and a full profile copied into each member's page body.
Profiles were COPIED (not linked) from the company Org Chart; never link back to it. Don't tag members by project.
Tom Hickie and Pinta Thunyalak have no Org Chart profile yet (no content / join date).
About page has an org chart: Manager → Product / Engineering / Quality.
- Francisco Rentería – Manager
- Tom Hickie – Engineer (frontend)
- Chinni Srikar – Engineer
- Zin WaiWai Nwe – Engineer
- Miri Den (田美里) – Project Manager (Product Manager role currently vacant; covered by Francisco)
- Pinta Thunyalak – QA

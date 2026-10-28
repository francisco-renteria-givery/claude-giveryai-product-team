# Givery AI Team – Notion workspace project

This project (and every session in it) works on the Givery AI Team Notion page.

- **Root page:** Givery AI Team
- **URL:** https://app.notion.com/p/givery/Givery-AI-Team-4076931cc44980768eb5cbaab4241568
- **Page ID:** `4076931cc44980768eb5cbaab4241568`
- Use the Notion MCP tools (`notion-fetch`, `notion-update-page`, `notion-create-pages`, `notion-create-database`) against this page ID.
- Goal: a team hub with members, news, team rules, and general information.

## Page structure
Hub navigation is the **Sections** database (inline gallery "Cards" on the root page),
data source `collection://e84d34fd-76a4-4504-ae76-8f21d9e3cff1` (props: Name, Tagline, Order).
Each section is a row in it:
- Team (row `4076931cc44981818098cd10351e5de6`) → contains Members database, data source `collection://1aff5912-2f89-477d-802d-f58f8a551cb9`
- News (row `4076931cc44981c69b97e12caf17354e`) → contains News & Announcements database, data source `collection://660f9819-3952-4879-9cdf-41bed05ac8d9`
- Meetings (row `4076931cc449818284e7c580a21f3cd1`) → contains Meetings & Rituals database, data source `collection://64078b8f-b1d3-486f-b0fb-bf44260d2119`
- Team Info – row/page `4076931cc449812eb6b0d2fec60e6360`
- Team Rules & Ways of Working – row/page `4076931cc4498105b618cd545fe311a2`
- Onboarding – row/page `4076931cc4498141ae87c958d65632c4`

Also on the root page:
- Communication section: Slack Channels database, data source `collection://3bfdf717-8b64-47f1-b95f-6cbd1ed35fc5` (giveryai_prod_* channels; "prod" = Product)
- Style: Givery brand (red #C80000 / black / white): red_bg banner callouts, red ● before headings, logo cover.

## Projects: link, never duplicate
The team has 2 projects, each with its own Notion page. The hub only links to them:
- 法務dx (Legal DX, TENA) – `4066931cc44980f8bddde488bc32ba2b`
- Givery AI Recorder – `3f36931cc44980ebb34fc1cdddb83673`
- Note: "Givery AI Home" (`36a6931cc449806dbbbae905a627aab2`) is NOT a project.

## Team members (6)
The Members database holds roles and basic info only. Don't tag members by project.
- Francisco Rentería – Manager
- Tom Hickie – Engineer (frontend)
- Chinni Srikar – Engineer
- Zin WaiWai Nwe – Engineer
- Miri Den (田美里) – Product Manager
- Pinta Thunyalak – QA

# GitLab Foundation AI for Economic Opportunity Fund Application

PolicyEngine's application to the GitLab Foundation AI for Economic Opportunity Fund.

## Grant Overview

- **Funder**: GitLab Foundation (in partnership with OpenAI)
- **Fund**: AI for Economic Opportunity Fund
- **Award**: $250,000 seed funding per project
- **Duration**: 6-month cohort (March - September 2026)
- **Concept Note Deadline**: October 31, 2025 (5:00 PM PT)
- **Application Type**: Two-stage (Concept Note, then Full Application if invited)

## Focus Areas

The fund seeks bold projects using AI to expand economic mobility and unlock economic opportunities. The foundation invites proposals that show how AI can meaningfully transform the systems that shape economic opportunity, including:

- Reimagining service delivery
- Unlocking new forms of personalized education and training
- Improving efficiency at scale
- Creating entirely new ways to connect people with income, skills, benefits, and opportunity

## Additional Support

Selected grantees receive:
- $250,000 in seed funding
- 6 months of technical support from OpenAI engineers and other experts
- OpenAI API credits
- Access to a network of leading practitioners and funders
- Opportunity to showcase work at Demo Day (August/September 2026 at OpenAI HQ)
- Eligibility for larger scaling capital through project partners

## Eligibility

- U.S.-based nonprofit organizations (programs can operate in non-U.S. markets)
- Partnerships between nonprofits and for-profit startups, consultants, and technology experts are encouraged
- For-profit social enterprises considered case-by-case with fiscal sponsor or nonprofit partner

## Previous Applications

PolicyEngine has previously applied to this fund:
- Solo application (2024)
- Joint application with Starlight (2024)

## Repository Structure

```
gitlab-ai-economic-opportunity-2025/
├── docs/                          # Application documents and responses
│   ├── concept-note/              # Concept note application (first stage)
│   │   ├── questions/             # Question structure and requirements
│   │   └── responses/             # Individual answer files
│   ├── full-application/          # Full application (if invited)
│   └── budget/                    # Budget documentation
├── materials/                      # Reference materials and grant documents
│   ├── grant-guidelines.md        # Official fund guidelines
│   ├── previous-solo-application.md      # Previous solo application
│   └── previous-starlight-joint.md       # Previous Starlight joint application
├── scripts/                        # Assembly and content management scripts
└── .github/                       # GitHub Actions for CI/CD
```

## Development

### Working on the Concept Note

Edit individual response files in `docs/concept-note/responses/`:

```bash
# Edit a specific response
code docs/concept-note/responses/project_summary.md

# Assemble and validate (if assembler script exists)
cd docs/concept-note
python3 assemble_concept_note.py
```

## Assessment Criteria

Based on GitLab Foundation's focus areas, applications are likely evaluated on:
- Innovation and transformative potential of AI solution
- Direct impact on economic mobility
- Feasibility and implementation plan
- Team expertise and capacity
- Alignment with focus areas (service delivery, education, efficiency, opportunity creation)
- Sustainability and scaling potential

## Key Dates

- **September 22, 2025**: Applications open
- **October 31, 2025**: Concept note deadline (5:00 PM PT)
- **November 14, 2025**: Finalist notifications
- **December 12, 2025**: Full application deadline (if invited)
- **December 2025 - January 2026**: Grantee selection
- **March 2026**: Cohort orientation begins
- **August/September 2026**: Demo Day at OpenAI HQ

## Links

- [AI for Economic Opportunity Fund](https://www.gitlabfoundation.org/futureofwork)
- [Fund Details](https://www.gitlabfoundation.org/partnerships/aifund)
- [PolicyEngine Website](https://policyengine.org)
- [PolicyEngine AI & Distributional Policy Research](https://policyengine.github.io/ai-growth-research/)

## PolicyEngine Context

PolicyEngine is a nonprofit building open-source tools to analyze the impacts of public policy on society. Our work directly addresses economic opportunity by:

- Making tax and benefit policy accessible and understandable
- Analyzing policy impacts on households across income distributions
- Supporting evidence-based policymaking
- Democratizing access to policy analysis tools
- Researching how policies mediate AI's distributional impacts

This application builds on our ongoing research into how economic policies shape the relationship between AI-driven economic shocks and distributional outcomes.

## Advisory Board

The fund's advisory board includes representatives from:
- Ballmer Group
- Gates Foundation
- OpenAI
- GitLab
- Other leading organizations in economic mobility and AI

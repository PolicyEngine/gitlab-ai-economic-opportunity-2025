# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository organizes PolicyEngine's application to the GitLab Foundation AI for Economic Opportunity Fund. The fund is a partnership between GitLab Foundation and OpenAI that seeks bold projects using AI to expand economic mobility.

## Previous Applications

PolicyEngine has previously applied to this fund:
- Solo application (2024) - focusing on PolicyEngine's AI-powered policy analysis tools
- Joint application with Starlight (2024) - partnership proposal for benefits access

## Grant Details

- **Award**: $250,000 seed funding per project
- **Total Fund**: Expected to exceed $10 million across all grantees
- **Concept Note Deadline**: October 31, 2025 (5:00 PM PT)
- **Finalist Notifications**: November 14, 2025
- **Full Application Deadline**: December 12, 2025 (if invited)
- **Grantee Selection**: December 2025 - January 2026
- **Cohort Duration**: March 2026 - September 2026
- **Focus**: Using AI to expand economic mobility

## Repository Structure

- `docs/`: Application documents and responses
  - `concept-note/`: Concept note application (first stage)
    - `questions/`: Question requirements and structure
    - `responses/`: Individual answer files (one per question)
  - `full-application/`: Full application (if invited after concept note)
  - `budget/`: Budget documentation
- `materials/`: Reference materials including grant guidelines and previous applications
- `scripts/`: Python scripts for content assembly and validation
- `.github/`: GitHub Actions for CI/CD

## Key Commands

### Content Assembly
```bash
# From docs/concept-note/ directory
python3 assemble_concept_note.py  # Assemble and validate concept note

# From root directory
python3 scripts/sync_content.py    # Sync content (if applicable)
```

## Development Workflow

### Making Content Changes

**IMPORTANT:** Edit source markdown files, then assemble/validate:

1. **Edit markdown source files** in `docs/concept-note/responses/*.md`
2. **Run assembly script** to generate complete concept note (if applicable)
3. **Review assembled output** for completeness and word counts
4. **Commit all changes** (both markdown sources and generated files)

### Key Files

**Source Files (edit these):**
- `docs/concept-note/responses/*.md` - Individual question responses
- `docs/budget/*.md` - Budget tables and justification

**Generated Files (do not edit directly):**
- `docs/concept-note/ASSEMBLED_CONCEPT_NOTE.md` - Auto-generated from responses (if applicable)

## Grant Focus Areas

Applications should demonstrate how AI can meaningfully transform systems that shape economic opportunity. The foundation is particularly interested in:

1. **Reimagining Service Delivery**
   - Using AI to improve how people access benefits, services, and resources
   - Streamlining enrollment and eligibility processes
   - Personalized guidance and support

2. **Unlocking Personalized Education and Training**
   - AI-powered skills development and career pathways
   - Adaptive learning and training programs
   - Skills matching and job placement

3. **Improving Efficiency at Scale**
   - Automating repetitive tasks to free up staff for high-touch work
   - Data-driven decision making
   - Resource optimization

4. **Creating New Pathways to Opportunity**
   - Novel approaches to connecting people with income, skills, benefits
   - New models for economic participation
   - Innovative solutions to structural barriers

## Content Development Guidelines

- Focus on how AI specifically advances economic mobility
- Demonstrate transformative potential, not incremental improvements
- Show clear connection between AI capabilities and economic outcomes
- Emphasize feasibility and realistic implementation
- Highlight team expertise in both AI and economic mobility
- Address technical approach, including use of OpenAI tools/APIs
- Include concrete success metrics and evaluation plans
- Show awareness of equity, ethics, and potential harms

## PolicyEngine Context

PolicyEngine is a nonprofit organization that builds open-source tools to analyze the impacts of public policy on society. Our work directly addresses economic mobility by:

- **Democratizing Policy Analysis**: Making complex tax-benefit modeling accessible to everyone
- **Evidence-Based Policymaking**: Providing data-driven insights for policy decisions
- **Household-Level Impact**: Showing how policies affect real families across income distributions
- **AI & Distributional Research**: Modeling how policies mediate AI's economic impacts
- **Open Source Infrastructure**: Building public goods for policy analysis

## U.S. Focus with Global Potential

While PolicyEngine operates in multiple countries (US, UK, Canada), this application should:
- Emphasize U.S.-based impact and operations
- Highlight U.S. partnerships and collaborations
- Focus on U.S. policy context and economic mobility challenges
- Note potential for global expansion where relevant

## Application Strategy

### Concept Note (Stage 1)
- Concise, compelling narrative
- Clear problem statement and AI solution
- Demonstrable impact on economic mobility
- Team credibility and capacity
- Realistic budget and timeline

### Full Application (Stage 2, if invited)
- Detailed technical approach
- Comprehensive evaluation plan
- Specific OpenAI API/tool usage
- Risk mitigation strategies
- Scaling and sustainability plans
- Partnership and collaboration details

## Assessment Criteria (Inferred)

Based on fund focus areas:
- **Innovation**: How transformative is the AI application?
- **Impact**: Direct connection to economic mobility outcomes
- **Feasibility**: Realistic plan, capable team, appropriate budget
- **AI Integration**: Thoughtful, strategic use of AI (not AI for AI's sake)
- **Equity**: Attention to serving underserved communities
- **Sustainability**: Path to continued impact beyond grant period
- **Scalability**: Potential to reach more people or replicate elsewhere

## Additional Support Benefits

Selected grantees receive:
- $250,000 seed funding
- 6 months of OpenAI engineer technical support
- OpenAI API credits
- Cohort-based peer learning
- Network access to practitioners and funders
- Demo Day platform at OpenAI HQ
- Eligibility for additional scaling capital

## Key Dates

- **September 22, 2025**: Applications open
- **October 31, 2025**: Concept note deadline (5:00 PM PT)
- **November 14, 2025**: Finalists notified
- **December 12, 2025**: Full applications due (if invited)
- **December 2025 - January 2026**: Grantee selection
- **March 2026**: Cohort orientation
- **August/September 2026**: Demo Day at OpenAI HQ

## Resources

- [AI for Economic Opportunity Fund Homepage](https://www.gitlabfoundation.org/futureofwork)
- [Fund Details and Requirements](https://www.gitlabfoundation.org/partnerships/aifund)
- [PolicyEngine AI Research](https://policyengine.github.io/ai-growth-research/)
- [PolicyEngine Website](https://policyengine.org)

## Collaboration Notes

This application may involve:
- Partnerships with other organizations (potential joint applications)
- Collaboration with OpenAI on technical approach
- Engagement with economic mobility practitioners
- Advisory input from policy experts

## File Naming Conventions

- Markdown: `snake_case.md`
- Python scripts: `snake_case.py`

## Deployment

- If a review site is created, it will auto-deploy to GitHub Pages on pushes to `main`
- CI/CD validates builds on pull requests

This repository provides a foundation for developing a comprehensive grant application to the GitLab Foundation AI for Economic Opportunity Fund.

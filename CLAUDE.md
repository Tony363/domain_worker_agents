# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This repository contains **10 domain-specific AI tooling research profiles** designed for understanding how different professional personas search for and evaluate AI tools. Each profile represents a distinct industry vertical with unique AI tooling requirements, search behaviors, and evaluation criteria.

## Architecture & Purpose

### Core Concept: Domain Worker Personas
Each markdown file represents a comprehensive research profile for a specific professional role:
- Healthcare Research Scientist
- Financial Risk Analyst
- Legal Contract Specialist
- E-commerce Marketing Manager
- Manufacturing Quality Engineer
- Content Creator/Journalist
- Educational Curriculum Designer
- Real Estate Investment Analyst
- Agricultural Technology Advisor
- Customer Support Operations Lead

### Profile Structure (Consistent Across All Files)
Each profile follows a standardized 5-section format:

1. **Persona Identity**: Name, role, industry, organization type, years of experience
2. **AI Tooling Preferences**: Primary categories (5), specific technical requirements (accuracy, integration, speed, compliance)
3. **Use Case Scenarios**: 5 detailed workflows with explicit search intent examples
4. **Tool Evaluation Criteria**: Critical requirements (non-negotiable), high priority, nice-to-have features
5. **Vector DB Metadata**: Structured JSON for semantic search optimization
6. **Exa.ai Search Instructions**: Primary queries, search filters, browser automation instructions

### Design Philosophy
- **Semantic Search Optimization**: Profiles are written to maximize vector database retrieval quality
- **Real-World Workflows**: Each use case reflects actual professional workflows with multi-step processes
- **Search Intent Modeling**: Explicit examples of how professionals would query for AI tools
- **Evaluation Frameworks**: Structured criteria with emoji indicators (✅ critical, ⚡ high priority, 💰 nice-to-have)

## Working with Profiles

### When Creating New Profiles
1. **Maintain Structural Consistency**: Follow the exact 6-section format (Persona Identity → AI Tooling Preferences → Use Case Scenarios → Tool Evaluation Criteria → Vector DB Metadata → Exa.ai Search Instructions)
2. **5 Use Cases Minimum**: Each profile must include 5 detailed scenarios with workflow steps and 3 search intent examples per scenario
3. **Industry-Specific Language**: Use domain terminology and technical precision appropriate to the profession
4. **Compliance Awareness**: Include regulatory requirements (HIPAA, GDPR, Basel III, FDA, etc.) relevant to the industry
5. **Integration Requirements**: Specify actual systems/platforms the persona uses (e.g., Epic/Cerner for healthcare, Bloomberg for finance)

### When Modifying Profiles
- **Preserve JSON Schema**: The vector DB metadata must maintain the exact field structure for consistency
- **Update Search Instructions**: If tooling categories change, update both the metadata and Exa.ai search queries
- **Maintain Evaluation Triad**: Keep the 3-tier evaluation system (Critical → High Priority → Nice-to-Have)
- **Workflow Accuracy**: Use realistic multi-step workflows with proper technical terminology

### Vector DB Metadata Schema
```json
{
  "persona_id": "unique_identifier_001",
  "industry": "industry_category",
  "role_category": "functional_role",
  "ai_tool_categories": ["category1", "category2", ...],
  "technical_expertise": "beginner|intermediate|advanced|expert",
  "priority_dimensions": ["dimension1", "dimension2", ...],
  "use_case_tags": ["tag1", "tag2", ...],
  "compliance_requirements": ["requirement1", "requirement2", ...],
  "integration_systems": ["system1", "system2", ...],
  "search_query_optimization": ["query_theme1", "query_theme2", ...]
}
```

## Key Patterns & Conventions

### Naming Convention
Files follow the pattern: `##_role_description.md` (e.g., `01_healthcare_research_scientist.md`)

### Emoji Usage in Evaluation Criteria
- ✅ = Critical/Non-Negotiable (security, compliance, accuracy)
- ⚡ = High Priority/Performance (speed, integration, analytics)
- 🎯 = Accuracy/Precision (benchmarks, validation)
- 📊 = Reporting/Analytics (dashboards, insights)
- 🤝 = Collaboration/Integration (multi-user, systems)
- 💰 = Cost/Pricing (budget considerations)
- 🚀 = Innovation/Speed (cutting-edge features)

### Search Intent Format
Each use case includes 3 search intent examples structured as:
```
- "keyword1 keyword2 keyword3 [domain context]"
- "tool_category use_case [compliance/technical requirement]"
- "technology_stack integration_need [industry vertical]"
```

## Domain Expertise Requirements

When working with these profiles, understand that each persona requires **deep domain knowledge**:

- **Healthcare**: HIPAA, FDA regulations, clinical trial protocols, EHR systems, medical terminology
- **Financial Services**: Basel III/IV, SEC compliance, risk modeling (VaR, stress testing), Bloomberg/Reuters integration
- **Legal**: Attorney-client privilege, due diligence workflows, case law research, contract lifecycle management
- **Manufacturing**: Six Sigma, ISO standards, predictive maintenance, IoT sensor data, quality control
- **Education**: Pedagogy, learning management systems, accessibility standards, assessment design
- **Agriculture**: Precision farming, crop yield optimization, sustainability metrics, agronomic data
- **Customer Support**: CSAT/NPS metrics, ticket deflection rates, workforce management, multilingual support

## Validation & Quality Checks

Before committing changes to any profile:

1. **Structural Integrity**: Verify all 6 sections are present and properly formatted
2. **JSON Validity**: Ensure the vector DB metadata is valid JSON with correct field names
3. **Search Intent Completeness**: Confirm each use case has exactly 3 search intent examples
4. **Compliance Accuracy**: Validate that regulatory requirements are current and correctly specified
5. **Integration Reality Check**: Verify that specified systems/platforms are widely used in that industry
6. **Technical Precision**: Ensure accuracy metrics, latency requirements, and benchmarks are realistic

## Use Cases for This Repository

This repository is designed to support:
- **AI Tool Recommendation Engines**: Vector search over persona profiles to match tools to user needs
- **Search Query Optimization**: Training data for understanding domain-specific AI tool search behavior
- **Market Research**: Understanding how different verticals evaluate and adopt AI tooling
- **Content Strategy**: Creating targeted content for specific professional personas
- **Product Development**: Identifying key features and requirements for domain-specific AI products

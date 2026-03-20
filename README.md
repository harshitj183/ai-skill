# Smart Instructions Library for AI Agents

[![npm version](https://img.shields.io/npm/v/smart-instructions-library-of-ai-skill.svg?style=for-the-badge&color=blue)](https://www.npmjs.com/package/smart-instructions-library-of-ai-skill)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

![Architecture Overview](assets/hero.png)

## Overview

The **Smart Instructions Library** is an enterprise-grade collection of hyper-specialized AI instructions, extracted and synthesized from leading technology organizations including Anthropic, Vercel, Stripe, Supabase, Microsoft, and HashiCorp. 

Modern Large Language Models (LLMs) often hallucinate library-specific APIs or invent out-of-date syntax. By injecting these curated "Mega-Skills" and "Master Roles" directly into your IDE or workspace, you constrain the AI's generation parameters strictly to industry-standard architectural patterns and up-to-date documentation.

---

## Installation

This package is distributed via the NPM registry and requires zero dependencies. Run the following installation command in the root directory of your project:

```bash
npx smart-instructions-library-of-ai-skill init
```

**Execution Result:**
1. Installs the `SKILL.md` Core Directive.
2. Extracts 8 Persona Directives to the `roles/` directory.
3. Extracts 17 Technical Directives to the `skills/` directory.

---

## System Architecture

The library is decoupled into three primary execution tiers:

### 1. The Core Directive (`SKILL.md`)
The orchestration layer. This document mandates the basal behavior of your Agent, enforcing principles such as determinism, strict JSON outputs, minimal latency, and zero conversational filler.

### 2. The Master Roles (`roles/`)
Behavioral personas designed to scope the AI's perspective. Included personas:
- `backend_expert.md`, `frontend_expert.md`, `gpt5_core.md`, `product_manager.md`, `security_auditor.md`, `technical_writer.md`, `ui_ux_designer.md`, `wisdom_extractor.md`

### 3. The Mega-Skills (`skills/`)
Hard technical constraints and code blueprints for immediate contextual parsing.
- **Infrastructure:** `mcp_master.md`, `hashicorp_terraform.md`, `azure_graph_integrator.md`, `antigravity_mastery.md`
- **Application Logic:** `react_best_practices.md`, `react_native_performance.md`, `playwright_testing.md`
- **Backend Services:** `supabase_architect.md`, `stripe_integration.md`, `openai_structured_outputs.md`
- **Orchestration:** `composio_integrator.md`, `sanity_architecture.md`, `vercel_cloudflare_deploy.md`, `github_automation.md`
- **Cognitive Optimization:** `prompt_reasoning_trees.md`, `letta_agent_memory.md`, `anthropic_documents.md`

---

## Implementation Guides

To achieve optimal results, you must invoke a "Role" and an associated "Skill" simultaneously in your prompt. Below are the execution patterns across widely used platforms:

### Cursor IDE Integration
Cursor processes `.cursorrules` globally.
1. Execute the `npx` init command.
2. Rename the generated `SKILL.md` to `.cursorrules`.
3. In Cursor Chat, utilize surgical file invocation via the `@` modifier.

**Example Prompt:**
> "@frontend_expert.md @react_best_practices.md Implement the new dashboard layout enforcing React Server Components."

### Anthropic Claude Code CLI
Claude Code recursively loads Markdown context within the working directory.
**Example Prompt:**
> "Load SKILL.md. Assume the parameters defined in roles/security_auditor.md. Conduct a vulnerability audit of my authentication service."

### GitHub Copilot (VS Code)
Copilot indexing relies on active buffer tabs. Keep required skills active in background tabs.
**Example Prompt:**
> "#file:supabase_architect.md Review my PostgreSQL migration script for row-level security compliance against the defined architecture."

### Default Web Interfaces (ChatGPT Pro, Claude Pro)
Attach `SKILL.md` directly into the "Custom Instructions" or "System Prompts" setting. Standardize your query by uploading `roles/backend_expert.md` and `skills/stripe_integration.md` alongside your objective.

---

## Contribution and Standardization

Contributions to expand the "Mega-Skill" index are highly encouraged. When submitting Pull Requests, ensure the instructions emphasize brevity, deterministic logic, and up-to-date integration models.

**License:** MIT

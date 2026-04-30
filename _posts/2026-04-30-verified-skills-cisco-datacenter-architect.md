---
layout: post
title: "Verified Claude Code Skills for Cisco Datacenter & AI Architects"
date: 2026-04-30
author: cpedrode
description: >
  A security-vetted selection of Claude Code skills for Cisco datacenter architects
  with an AI background. Each skill was evaluated for source trust, GitHub signals,
  and SKILL.md content before being included.
tags:
  - claude-code
  - skills
  - cisco
  - datacenter
  - infrastructure
  - security
  - ai
  - terraform
  - kubernetes
---

# Verified Claude Code Skills for Cisco Datacenter & AI Architects

> **TL;DR** — The Claude Code skills ecosystem has a serious supply chain problem.
> Snyk's [ToxicSkills study (Feb 2026)](https://snyk.io/blog/toxicskills-malicious-ai-agent-skills-clawhub/)
> found prompt injection in **36%** of publicly available skills and **1,467 malicious payloads**
> across 3,984 scanned skills. This post only lists skills that passed a manual security filter.

---

## Security Filter Applied

Every skill below was evaluated against the following criteria before being listed:

| Signal | What Was Checked |
|---|---|
| **Source trust** | First-party (Anthropic) > Known org > Community 1k+ stars |
| **GitHub signals** | Stars, forks, account age, contributor diversity |
| **SKILL.md content** | Grep for `http`, `curl`, `env`, `base64`, hidden unicode, broad trigger conditions |
| **MCP servers** | Any bundled MCP server URL verified against a known organization |
| **Known flags** | Cross-referenced against Snyk ToxicSkills findings |

If a skill didn't pass all five checks, it was excluded — regardless of how useful it looked.

---

## Verified Stack

### Tier 1 — First-Party & Known Organizations

#### [anthropics/skills](https://github.com/anthropics/skills) · Official Anthropic · `10/10`

The safest starting point. Published and maintained by Anthropic. Apache 2.0 licensed.
No community repo risks. Read each SKILL.md anyway — good habit.

| Skill | Use Case |
|---|---|
| `claude-api` | Build, debug, and optimize Claude API / Anthropic SDK apps |
| `skill-creator` | Guided Q&A to scaffold new skills correctly |
| `webapp-testing` | Browser-based end-to-end testing automation |
| `mcp-builder` | Build MCP servers safely with guardrails |

**Relevant for:** AI development work, building internal tooling on the Claude API.

---

#### [trailofbits/skills](https://github.com/trailofbits/skills) · Trail of Bits · ⭐ 4.9k · `9/10`

Trail of Bits is one of the most respected security research firms in the industry —
authors of Slither, Echidna, publications on supply chain security, and CVE disclosures
going back over a decade. Their skills are narrow, well-documented, and transparent.

| Skill | Use Case |
|---|---|
| `audit-context-building` | Structured security audit methodology with line-by-line code analysis |
| `agentic-actions-auditor` | Scans GitHub Actions YAML for AI agent injection vulnerabilities |
| `testing-handbook-skills` | AppSec testing workflows from their published Testing Handbook |

**Relevant for:** Security audit workflows, CI/CD pipeline hardening, code review.

---

#### [antonbabenko/terraform-skill](https://github.com/antonbabenko/terraform-skill) · Anton Babenko · ⭐ 1.8k · `9/10`

Anton Babenko is a verified public figure in the Terraform community — author of modules
with over 100 million downloads, long-time HashiCorp community ambassador. The skill is
short, transparent, and grounded in official documentation.

| Skill | Use Case |
|---|---|
| `terraform-skill` | Terraform/OpenTofu best practices, module patterns, CI/CD, production IaC |

**Relevant for:** Datacenter infrastructure provisioning, network-as-code workflows.

---

### Tier 2 — Community, High Scrutiny, Narrow Scope

> **Before installing:** Open the raw SKILL.md on GitHub and run this check yourself:
> ```bash
> grep -iE "http|curl|fetch|base64|eval|\$[A-Z_]{3,}" SKILL.md
> ```
> If anything returns that isn't clearly documented behavior, don't install.

#### [LukasNiessen/terrashark](https://github.com/LukasNiessen/terrashark) · `7/10`

Addresses a real problem: LLMs hallucinate Terraform syntax. TerraShark grounds Claude
in official HashiCorp documentation. The SKILL.md is 79 lines — readable in under two
minutes. No network calls, no environment variable references.

**Relevant for:** Any Terraform/OpenTofu work in datacenter provisioning pipelines.

---

#### [LukasNiessen/kubernetes-skill](https://github.com/LukasNiessen/kubernetes-skill) · `7/10`

Same author and same approach as TerraShark, applied to Kubernetes and Helm.
Bakes in security contexts (`runAsNonRoot`, resource limits, liveness probes) by default.

**Relevant for:** Container workloads in the datacenter, Kubernetes cluster management.

---

## Skills to Skip

These were excluded despite appearing frequently in search results:

| Skill / Repo | Reason Excluded |
|---|---|
| Any skill from ClawHub or skills.sh marketplaces | 36% prompt injection rate (Snyk ToxicSkills) |
| `mukul975/Anthropic-Cybersecurity-Skills` | "Anthropic" in the name is **not** Anthropic — misleading branding |
| `pitimon/claude-cybersecurity-skill` | Unknown org, no track record, bilingual obfuscation risk |
| `alirezarezvani/claude-skills` (232+ skills) | Surface too large to vet individually |
| `Masriyan/Claude-Code-CyberSecurity-Skill` | Unknown author, no verifiable identity |
| Any skill bundling an MCP server from an unknown org | MCP poisoning vector — server runs with full tool privileges |

---

## What's Still Missing

No verified public skills exist for:

- **Cisco IOS / NX-OS / ASA** — config diffing, compliance checking, CVE-to-config mapping
- **Cisco ACI / APIC** — policy automation
- **Cisco DNA Center / Catalyst Center** — API workflows
- **Cisco ISE** — policy review and audit

These are the highest-value skills for a Cisco datacenter architect and the safest option
is to write them yourself — you control the content and there's no supply chain risk.

---

## How to Audit Any Skill Before Installing

Five-minute checklist before adding any skill:

1. **Read the raw SKILL.md** — not the rendered preview, the raw file
2. **Grep for red flags** — `http`, `curl`, `fetch`, `base64`, `eval`, `$ENV_VAR`
3. **Check trigger conditions** — overly broad triggers ("when user opens any URL") are a red flag
4. **Verify any MCP server URLs** — resolve the domain, confirm it belongs to a known org
5. **Sandbox first** — install in a throwaway environment with no real credentials before using in production

If the skill doesn't pass all five in under five minutes, the alternative is to write your own.
SKILL.md files are simple markdown — for common use cases, writing one takes less time than auditing a suspicious one.

---

## References

- [Snyk ToxicSkills Study](https://snyk.io/blog/toxicskills-malicious-ai-agent-skills-clawhub/)
- [Repello AI — How to Audit Any Claude Skill](https://repello.ai/blog/claude-code-skill-security)
- [Trail of Bits Skills Repository](https://github.com/trailofbits/skills)
- [Anthropic Official Skills Repository](https://github.com/anthropics/skills)
- [Anton Babenko Terraform Skill](https://github.com/antonbabenko/terraform-skill)
- [SecurityWeek — Claude Code Prompt Injection via Comments](https://www.securityweek.com/claude-code-gemini-cli-github-copilot-agents-vulnerable-to-prompt-injection-via-comments/)
- [Anthropic Agent Skills Documentation](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview)

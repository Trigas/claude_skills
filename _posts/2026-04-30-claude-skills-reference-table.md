---
layout: single
title: "Claude Code Skills — Full Reference Table"
date: 2026-04-30
author_profile: true
read_time: true
show_date: true
toc: true
toc_sticky: true
toc_label: "Categories"
categories:
  - Reference
tags:
  - claude-code
  - skills
  - reference
  - security
  - cisco
excerpt: >
  Complete reference table of all Claude Code skills identified — vetted, pending, and flagged.
  Batch validation in progress. Companion to the verified skills post.
---

# Claude Code Skills — Full Reference Table

> Companion to: [Verified Claude Code Skills for Cisco Datacenter & AI Architects](/claude_skills/2026/04/30/verified-skills-cisco-datacenter-architect.html)

This table covers **every skill identified** during research — vetted, pending validation, and flagged.
Batch validation is in progress. Check back as scores and statuses are filled in.

---

## Status Legend

| Badge | Meaning |
|---|---|
| ✅ **Vetted** | Source verified, SKILL.md reviewed, no red flags |
| ⏳ **Pending** | Not yet reviewed — do not install before validating |
| ❌ **Skip** | Failed one or more security checks |

**Score** = 1–10 · Source trust (40%) + GitHub signals (20%) + SKILL.md transparency (20%) + Relevance (20%)  
`—` = not yet scored

---

## Official / Anthropic

| Skill | Summary | Link | ⭐ | Status | Score |
|---|---|---|---|---|---|
| `claude-api` | Build, debug, optimize Claude API / Anthropic SDK apps | [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/claude-api) | — | ✅ | 10/10 |
| `skill-creator` | Guided Q&A to scaffold new skills correctly | [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/skill-creator) | — | ✅ | 10/10 |
| `webapp-testing` | Browser-based end-to-end testing automation | [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/webapp-testing) | — | ✅ | 10/10 |
| `mcp-builder` | Build MCP servers with built-in guardrails | [anthropics/skills](https://github.com/anthropics/skills/tree/main/skills/mcp-builder) | — | ✅ | 10/10 |

---

## Security & Audit

| Skill | Summary | Link | ⭐ | Status | Score |
|---|---|---|---|---|---|
| `audit-context-building` | Structured security audit — line-by-line code analysis | [trailofbits/skills](https://github.com/trailofbits/skills/tree/main/plugins/audit-context-building) | 4.9k | ✅ | 9/10 |
| `agentic-actions-auditor` | Scans GitHub Actions YAML for AI agent injection vulns | [trailofbits/skills](https://github.com/trailofbits/skills/tree/main/plugins/agentic-actions-auditor) | 4.9k | ✅ | 9/10 |
| `testing-handbook-skills` | AppSec testing from Trail of Bits Testing Handbook | [trailofbits/skills](https://github.com/trailofbits/skills/tree/main/plugins/testing-handbook-skills) | 4.9k | ✅ | 9/10 |
| `claude-cybersecurity-skill` | 18 domains: IR, DFIR, OT/ICS, Zero Trust, Cloud/CSPM | [pitimon](https://github.com/pitimon/claude-cybersecurity-skill) | ⏳ | ⏳ | — |
| `cybersecurity-claude-skills` | Web hacking, pentest recon, secure code review, CTF | [mahmutka](https://github.com/mahmutka/cybersecurity-claude-skills) | ⏳ | ⏳ | — |
| `Claude-Code-CyberSecurity-Skill` | 15 skills: offensive/defensive, threat hunting, CSOC | [Masriyan](https://github.com/Masriyan/Claude-Code-CyberSecurity-Skill) | ⏳ | ❌ | — |
| `Anthropic-Cybersecurity-Skills` | 754 skills, MITRE ATT&CK mapped — misleading name | [mukul975](https://github.com/mukul975/Anthropic-Cybersecurity-Skills) | ⏳ | ❌ | — |

---

## Infrastructure as Code

| Skill | Summary | Link | ⭐ | Status | Score |
|---|---|---|---|---|---|
| `terraform-skill` | Terraform/OpenTofu best practices, modules, CI/CD | [antonbabenko](https://github.com/antonbabenko/terraform-skill) | 1.8k | ✅ | 9/10 |
| `terrashark` | Eliminates Terraform hallucinations, grounded in HashiCorp docs | [LukasNiessen](https://github.com/LukasNiessen/terrashark) | ⏳ | ⏳ | 7/10 |
| `devops-skills` | Terraform/OpenTofu workflows, AWS infra, safety-first IaC | [lgbarn](https://github.com/lgbarn/devops-skills) | ⏳ | ⏳ | — |

---

## Container & Orchestration

| Skill | Summary | Link | ⭐ | Status | Score |
|---|---|---|---|---|---|
| `kubernetes-skill` | Eliminates K8s hallucinations, security contexts baked in | [LukasNiessen](https://github.com/LukasNiessen/kubernetes-skill) | ⏳ | ⏳ | 7/10 |
| `claude-code-docker-skill` | Container-based dev, run commands inside Docker | [wrsmith108](https://github.com/wrsmith108/claude-code-docker-skill) | ⏳ | ⏳ | — |

---

## GitHub / CI-CD Automation

| Skill | Summary | Link | ⭐ | Status | Score |
|---|---|---|---|---|---|
| `claude-code-showcase` | GitHub Actions workflows, PR automation, code review hooks | [ChrisWiles](https://github.com/ChrisWiles/claude-code-showcase) | ⏳ | ⏳ | — |
| `claude-bitbucket-devops-skill` | Bitbucket DevOps automation workflows | [Apra-Labs](https://github.com/Apra-Labs/claude-bitbucket-devops-skill) | ⏳ | ⏳ | — |
| `claude-skills` (232+) | Broad: GitHub automation, compliance, Jira/Confluence MCP | [alirezarezvani](https://github.com/alirezarezvani/claude-skills) | 5.2k | ❌ | — |

---

## AI / Claude API Development

| Skill | Summary | Link | ⭐ | Status | Score |
|---|---|---|---|---|---|
| `claude-code-skills` | Full delivery lifecycle + hex-ssh MCP (remote SSH) | [levnikolaevich](https://github.com/levnikolaevich/claude-code-skills) | ⏳ | ⏳ | — |
| `claude-skills` (enhanced AI) | Enhanced AI workflows, prompt engineering | [glebis](https://github.com/glebis/claude-skills) | ⏳ | ⏳ | — |
| `scientific-agent-skills` | Research, engineering, analysis, finance, writing | [K-Dense-AI](https://github.com/K-Dense-AI/claude-scientific-skills) | ⏳ | ⏳ | — |

---

## Large Collections (Vet Individually)

| Collection | Skills Count | Summary | Link | ⭐ | Status |
|---|---|---|---|---|---|
| `awesome-claude-skills` | 1000+ | Curated index — links only, not skills themselves | [travisvn](https://github.com/travisvn/awesome-claude-skills) | ⏳ | ⏳ |
| `awesome-claude-skills` | 1000+ | Alternative curated index | [ComposioHQ](https://github.com/ComposioHQ/awesome-claude-skills) | ⏳ | ⏳ |
| `awesome-agent-skills` | 1000+ | Cross-platform: Claude, Codex, Gemini, Cursor | [VoltAgent](https://github.com/VoltAgent/awesome-agent-skills) | ⏳ | ⏳ |
| `antigravity-awesome-skills` | 1400+ | Installable library with CLI installer | [sickn33](https://github.com/sickn33/antigravity-awesome-skills) | ⏳ | ❌ |
| `claude-skills` | 232+ | Engineering, compliance, C-level advisory | [alirezarezvani](https://github.com/alirezarezvani/claude-skills) | 5.2k | ❌ |

> ⚠️ Large collections cannot be vetted as a unit. If installing from these, pick individual skills and validate each one separately using the checklist below.

---

## Cisco-Specific Gap (Nothing Public Exists)

| Domain | What's Needed |
|---|---|
| **IOS / NX-OS / ASA** | Config diffing, CVE-to-config mapping, compliance audit |
| **ACI / APIC** | Policy automation, tenant/EPG workflow |
| **DNA Center / Catalyst Center** | REST API automation, intent-based networking |
| **ISE** | Posture audit, RBAC analysis, policy review |

These require custom skills — writing your own is also the safest option.

---

## Batch Validation Script

Run this for every ⏳ entry to fill in the blanks:

```bash
#!/bin/bash
OWNER=$1
REPO=$2

echo "=== $OWNER/$REPO ==="

# Stars & account age
gh api repos/$OWNER/$REPO --jq '"Stars: \(.stargazers_count) | Created: \(.created_at)"'
gh api users/$OWNER --jq '"Account created: \(.created_at)"'

# Fetch SKILL.md (try common paths)
for path in SKILL.md skills/*/SKILL.md plugins/*/SKILL.md; do
  URL="https://raw.githubusercontent.com/$OWNER/$REPO/main/$path"
  curl -sf "$URL" -o /tmp/skill_audit.md && break
done

# Red flag grep
echo "--- Red flags ---"
grep -inE "http[s]?://|curl |fetch\(|base64|eval\(|\\\$[A-Z_]{3,}|ignore previous|do not tell|hidden:" /tmp/skill_audit.md || echo "None found"

# Hidden unicode
echo "--- Unicode check ---"
python3 -c "
data = open('/tmp/skill_audit.md').read()
hits = [(i, hex(ord(c))) for i, c in enumerate(data) if ord(c) > 127 and ord(c) not in range(0x2018, 0x201F)]
print(hits[:10] if hits else 'Clean')
"
```

Usage: `bash validate.sh trailofbits skills`

---

## References

- [Snyk ToxicSkills Study](https://snyk.io/blog/toxicskills-malicious-ai-agent-skills-clawhub/)
- [Repello AI — Skill Audit Guide](https://repello.ai/blog/claude-code-skill-security)
- [Anthropic Skills Documentation](https://platform.claude.com/docs/en/agents-and-tools/agent-skills/overview)

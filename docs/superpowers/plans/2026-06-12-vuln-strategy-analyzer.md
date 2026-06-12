# vuln-strategy-analyzer Skill Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create the vuln-strategy-analyzer skill file as a self-contained SKILL.md.

**Architecture:** Single SKILL.md file placed in `/root/.config/opencode/skills/vuln_hunt/vuln-strategy-analyzer/SKILL.md`, alongside existing vuln_hunt skills. The skill uses a 4-layer analysis pipeline to classify user tasks and output structured strategy plans.

**Tech Stack:** Markdown (SKILL.md format for opencode)

---

### Task 1: Create the skill directory and SKILL.md

**Files:**
- Create: `/root/.config/opencode/skills/vuln_hunt/vuln-strategy-analyzer/SKILL.md`

- [ ] **Step 1: Create skill directory**

Run: `mkdir -p /root/.config/opencode/skills/vuln_hunt/vuln-strategy-analyzer`

- [ ] **Step 2: Write SKILL.md with full content**

The SKILL.md must contain:

1. **YAML frontmatter** — name: `vuln-strategy-analyzer`, description for explicit on-demand trigger
2. **Overview** — self-contained strategy planner, only outputs plans
3. **4-Layer Architecture** — Input Form Recognition → Intent Classification → Methodology Selection → Scenario Refinement
4. **Layer 1: Input Form Recognition** — table mapping detection rules
5. **Layer 2: Intent Classification** — 10 categories with trigger conditions
6. **Layer 3: Methodology Selection** — per-intent mapping with reasoning
7. **Layer 4: Scenario Refinement** — 10+ predefined scenario templates, fallback to decision tree
8. **Methodology Reference** — top-down / bottom-up / hybrid details
9. **Output Schema** — A-F six sections, directory `.vuln_strategy/`, file naming convention
10. **Scenario Guidance** — 5 scenario categories with methodology mapping
11. **Workflow** — steps from user invocation to plan output
12. **Constraints** — what the skill does NOT do

- [ ] **Step 3: Verify structure**

Run: `head -5 /root/.config/opencode/skills/vuln_hunt/vuln-strategy-analyzer/SKILL.md`
Expected: YAML frontmatter with `name: vuln-strategy-analyzer`

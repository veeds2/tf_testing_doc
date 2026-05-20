# TestFactors Documentation — Authoring Guide

Documentation site for [TestFactors](https://testfactors.com) — AI-powered testing for HR systems.

- Pages are MDX with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally
- Run `mint broken-links` to check links before pushing

## Audience

End users — HR analysts, HRIS specialists, business analysts, testers. **Not engineers.** If a sentence assumes technical context, rewrite it.

## Terminology

Use these exact terms (consistency matters for search and SEO):

- **Workspace** (not "tenant", "account")
- **Project** (a container of workbooks + scenarios + test artifacts)
- **Workbook** (an uploaded `.xlsx` HR spec)
- **Scenario** (what we want to test)
- **Test case** (a specific situation within a scenario)
- **Test script** (the step-by-step instructions a tester follows)
- **Member** (not "user"; "user" is too generic)
- **Role**: `Owner`, `Admin`, `Member`, `Viewer`
- **FactorBot** (the in-app AI chat)

## Style preferences

- Active voice, second person ("you")
- One idea per sentence
- Sentence case for headings
- **Bold** for UI elements: Click **Settings → Members**
- Backticks for file names, paths, and code: `docs.json`, `.xlsx`
- Use Mintlify components (`<Steps>`, `<Card>`, `<Tip>`, `<Note>`, `<Accordion>`) liberally — they're what make the site feel polished
- Never expose internal jargon (Lovable, Rails, AASM, Solid Queue, etc.)

## Page template (use for every module guide)

```
---
title: "<Module name>"
description: "<One-line value prop>"
icon: "<lucide-icon-name>"
---

## What this module does
## Who uses it
## Before you start
## Step-by-step (Mintlify <Steps>)
## Tips
## Troubleshooting (Mintlify <AccordionGroup>)
## Related guides (Mintlify <CardGroup>)
```

## Content boundaries

- ✅ User-facing features, workflows, settings the user can see and control
- ✅ Permissions and role behavior
- ✅ Integrations the user configures themselves
- ❌ Internal architecture (Rails models, AASM states, job queues)
- ❌ Developer/Lovable integration docs (those live in the private `ba_testing_api` repo)
- ❌ Anything tied to an internal Jira ticket or sprint plan

## Adding a new page

1. Create the `.mdx` file under `platform/`, `knowledge-ai/`, or `admin/`
2. Add its path to the correct `pages:` array in `docs.json`
3. Run `mint dev` locally to verify
4. Open a PR

## Adding screenshots

- Save under `/images/<module>/<descriptive-name>.png`
- Use `![Alt text describing what the screenshot shows](/images/<module>/<filename>.png)`
- Prefer PNG with transparent background where possible

# SkillPi — Find AI Agent Skills, Safely

**The free skill-scout for Claude Code, Cursor, Codex and every SKILL.md-compatible agent. Describe the job — SkillPi finds, vets and recommends the right agent skill, with install commands.**

`find-skills` made you browse a leaderboard. SkillPi scouts for you: tell your agent what you're trying to do — "grow my TikTok", "automate my store's content", "audit this repo" — and it searches SkillPi (https://skillpi.com) and the open registries (skills.sh, ClawHub), checks every candidate for safety, permissions and freshness, and hands you a short ranked list with one clear recommendation.

## Why SkillPi

- One command, any skill — you describe an outcome, not a keyword
- Vetted, not just listed — every pick passes a permission review; skills that grab credentials, browser cookies or wallet keys get flagged, never recommended
- Curated picks first — security-scanned skills and scenario bundles from the SkillPi marketplace (TikTok Creator Pack, Indie Store Seller Pack…) surface first when they fit
- Free forever — discovery should be free; that's the whole point

## SkillPi vs find-skills

|  | find-skills | SkillPi |
|---|---|---|
| Ranking logic | Install counts & author reputation | Installs plus permission & safety vetting |
| Sources | skills.sh registry | SkillPi marketplace + skills.sh + ClawHub |
| Curated bundles | ✗ | ✓ Scenario packs (creator, seller, marketer…) |
| Security stance | Trust the popular ones | Inspect first; credentials-touching = hard no |
| Price | Free | Free |

## What SkillPi checks before recommending a skill

1. Permissions — does it touch ~/.ssh, browser cookies, API tokens, wallet keys, or upload data to unknown domains?
2. Freshness — maintained within the last 6 months beats abandoned
3. Signal — installs, downloads and stars relative to its category
4. Fit — the skill's actual instructions match the job you described

## Use cases

- Content & social media — TikTok/Reels scripting, hook analysis, posting checklists
- E-commerce — Shopify product descriptions, review replies, store audits
- Marketing — SEO audits, competitor content-gap analysis, ad creative
- Coding — code review, testing, deployment and documentation skills
- Productivity — email drafting, meeting notes, spreadsheet automation

## Install

With the skills CLI:

    npx skills add Findskills/skillpi

Or manually — clone this repo into your agent's skills directory:

    git clone https://github.com/Findskills/skillpi ~/.claude/skills/skillpi

Works with Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI and other agents that support the open SKILL.md standard.

## Use it

Just tell your agent what you're trying to do:

> "SkillPi, find me something that turns my product photos into TikTok posts."
> "Is there a skill that audits a landing page for conversion?"
> "Find me a skill that drafts replies to customer emails."

## FAQ

Is SkillPi free?
Yes. The discovery skill is free and MIT-licensed. Some skills it recommends are paid — it always tells you which and why before you install anything.

How is this different from find-skills?
find-skills ranks by popularity. SkillPi ranks by popularity and trust: every recommendation is permission-checked, and curated, security-scanned picks from the SkillPi marketplace come first when they fit.

Is it safe to install skills recommended here?
Safer than picking from a raw registry — roughly 12% of skills on open registries have been caught behaving maliciously (credential theft, data exfiltration). SkillPi flags those patterns instead of recommending them. Still read any skill before installing it in a production environment.

Which agents does it work with?
Any agent supporting the SKILL.md standard, including Claude Code, Codex, Cursor, GitHub Copilot and Gemini CLI.

## About SkillPi

SkillPi is the free discovery skill from SkillPi (https://skillpi.com) — one marketplace, infinite skills. Every skill sold on SkillPi passes a security scan and declares its permissions on the product page, because trust is the product.

⭐ Star this repo if SkillPi found you a good skill — it helps other builders discover it too.

MIT licensed. PRs and skill suggestions welcome.

Keywords: agent skills, claude skills, claude code skills, ai agent skills finder, find skills, skill marketplace, SKILL.md, ai tools, agent automation, cursor skills, codex skills

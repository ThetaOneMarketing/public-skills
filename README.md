# Skills

Free skills by Joey Farbstein. Human page: [joeyfarbstein.com/skills](https://joeyfarbstein.com/skills).

## For contractors and home service owners: audit your own marketing

Start with **ask-joey**: tell it what's going on with your marketing and it
tells you which audit to run first, and answers marketing questions the way
Joey would.

Then three audits. Each one is a file you hand to an AI that can drive a
browser (Claude on the desktop app, Claude in Chrome, or ChatGPT in agent
mode). The AI opens the real screens, takes screenshots, and hands back one
page of findings. It never changes anything.

| Skill | What it does | Login needed |
|---|---|---|
| **ask-joey** | The front door. Two or three questions, then which audit to run and in what order. Also answers marketing questions using Joey's rules. | None. Works in a plain chat. |
| **website-audit** | Your site on a phone: can they call, does the form land, a page per service and town, speed, trust, tracking. | None |
| **local-seo-audit** | Your Google listing (the map) and the regular results: category, reviews, phone match, where you show up for each service in each town, and who's beating you. | None. Google sign-in adds your listing's call counts and Search Console. |
| **google-ads-audit** | Where the ad money went: what counts as a lead, location and network settings, the search terms report, wasted spend, auto-apply, who owns the account. | Signed in to Google Ads, read access is enough. |

### Run one in ChatGPT or Claude (no install)

Open the skill file, copy all of it, paste it as the first message in a new
chat in Claude (desktop app or Chrome) or ChatGPT agent mode. Send. It asks
for your website or business name and goes.

- [skills/ask-joey/SKILL.md](skills/ask-joey/SKILL.md)
- [skills/website-audit/SKILL.md](skills/website-audit/SKILL.md)
- [skills/local-seo-audit/SKILL.md](skills/local-seo-audit/SKILL.md)
- [skills/google-ads-audit/SKILL.md](skills/google-ads-audit/SKILL.md)

### Install in Claude Code

```
npx skills@latest add ThetaOneMarketing/skills --skill=ask-joey
npx skills@latest add ThetaOneMarketing/skills --skill=website-audit
npx skills@latest add ThetaOneMarketing/skills --skill=local-seo-audit
npx skills@latest add ThetaOneMarketing/skills --skill=google-ads-audit
```

Or all four as one plugin that updates when I ship:

```
claude plugin marketplace add ThetaOneMarketing/skills && claude plugin install ask-joey@joey
```

Then type `/ask-joey`, `/website-audit`, `/local-seo-audit`, or `/google-ads-audit`.

The fourth audit, **Where You Stand with AI** (how you already use AI, and
what to set up tonight), lives in
[ThetaOneMarketing/joeyfarbstein-ai](https://github.com/ThetaOneMarketing/joeyfarbstein-ai).

## For people who build with AI

| Skill | What it does | Lives in |
|---|---|---|
| **raise-the-bar** | The AI can't grade its own work. Before it says "done", a fresh critic that sees only your ask and the finished work says SHIP or NOT YET, and names the one thing to fix. Three rounds at most. | this repo |
| **hatch** | Turns a fuzzy idea or risky decision into a clear, defended result. Six stages: frame, diverge, judge, red-team, build, ship-gate. | [ThetaOneMarketing/hatch](https://github.com/ThetaOneMarketing/hatch) |

```
npx skills@latest add ThetaOneMarketing/skills --skill=raise-the-bar
claude plugin marketplace add ThetaOneMarketing/hatch && claude plugin install hatch@hatch
```

## License

MIT. Credits are in [ATTRIBUTION.md](ATTRIBUTION.md).

Made by [Joey Farbstein](https://joeyfarbstein.com).

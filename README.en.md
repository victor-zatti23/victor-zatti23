# Victor Zatti

[Português](README.md) · **English**

**A QA engineer who automates QA with AI.** I test investment platforms (web, API and mobile) and build the tools that decide *what* to test, *how* to prove it passed and *where* to record the evidence.

More and more code is written by AI, and it ships faster than anyone can review by hand. My job is to keep testing at that pace without losing sight of the acceptance criteria.

---

### What I do

- **Risk-based QA**: I read what was merged each day and rank it by what could break production, not by arrival order.
- **Web and API automation**: Playwright with real login (Keycloak), saved sessions and assertions against the API instead of trusting the screen alone.
- **Mobile**: test scripts on the iOS simulator and on physical Android devices with Maestro, with a screenshot of every step as evidence.
- **AI agents in the workflow**: Claude Code skills that turn a plain-language bug report into a structured ticket, run test scripts and produce the final PDF report.
- **Multi-agent development**: orchestrator + backend dev + frontend dev + reviewer, with QA kept independent as the exit gate.

### Projects

| Project | What it solves |
|---|---|
| [qa-risk-queue](https://github.com/victor-zatti23/qa-risk-queue) | In a pipeline that went from 19 to 803 PRs/month, most merged without approval, it answers one question every day: *what should I test today?* Scores each change by its nature (prod, authorization, contract, config) and groups by ticket. |
| playwright-qa-harness _(coming soon)_ | Web QA harness: login, test account provisioning, API as the oracle and an HTML report with screenshots. |
| mobile-qa-maestro _(coming soon)_ | Maestro flows for iOS and Android, running on simulators and real devices. |
| claude-qa-skills _(coming soon)_ | Claude Code skills for QA: bug → structured ticket, test plans, daily PDF report. |
| multi-agent-dev-flow _(coming soon)_ | How I built a team of agents (Opus + Sonnet) to implement tickets, with real cost, what the reviewer caught and the gates that keep CI green. |

### Tools

`Playwright` · `Maestro` · `Cypress` · `Postman` · `SQL` · `Node.js` · `GitHub API (GraphQL)` · `Jira` · `Azure DevOps` · `Claude Code` · `AI agents / MCP`

### How I think about testing

- The screen is not the oracle. If the API or the database says otherwise, the screen is lying.
- Every case has evidence: a screenshot of the step, not "tested and it passed".
- AI already writes the unit tests. The gap is in acceptance criteria, integration between screens and configuration parity across environments.


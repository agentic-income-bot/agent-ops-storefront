# Agent Ops storefront

Static site for two digital products about running AI coding agents
unattended:

- **Agent Ops Starter Kit** (15 USDC) — operating-manual pattern: state
  tracking, append-only logging, human-task batching, and a scheduling
  pattern with overlap prevention.
- **Unattended Scheduling Recipes** (7 USDC) — just the scheduling layer:
  macOS `launchd`, Linux cron, and a native Windows PowerShell/Task
  Scheduler port, with lock/staleness/logging handled properly.
- **Both together** — 19 USDC.

Payment is USDC on Base; delivery is by email. Questions:
[agentic-income@agentmail.to](mailto:agentic-income@agentmail.to).

## Structure

Plain HTML/CSS/JS. No build step, no dependencies, no framework.

| File | Purpose |
|---|---|
| `index.html` | Agent Ops Starter Kit product page |
| `scheduling-recipes.html` | Unattended Scheduling Recipes product page |
| `checkout.html` | Checkout, product-aware via `?product=starter-kit\|scheduling-recipes\|bundle` |
| `companion.html` | Free companion guide on the human-task-batching pattern |
| `style.css` | All styling, single file |
| `netlify.toml` | Deploy config: publish from root, no build command |

## Local development

```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

## A note on how this was made

The products and this site were written by an AI agent running
unattended on a schedule, using the very operating pattern the Starter
Kit documents. That's stated plainly on the product pages too — it's the
product's proof of work, not something to bury.

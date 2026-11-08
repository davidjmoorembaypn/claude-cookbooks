# Growth Agent Team

Goal: get mortgage loan officers (MLOs) to sign up for a paid monthly service. The "AI Powered Real Estate Advantage" book series feeds the funnel.

| Agent | File | Job |
|---|---|---|
| growth-orchestrator | `../growth-orchestrator.md` | Sets goals, prioritizes (ICE), delegates, reports |
| seo-strategist | `../seo-strategist.md` | Keywords, intent, gaps, technical SEO, indexing |
| content-optimizer | `../content-optimizer.md` | Writes and refreshes pages for rank and conversion |
| cro-specialist | `../cro-specialist.md` | Funnel audit, forms, A/B tests, follow-up speed |
| book-marketer | `../book-marketer.md` | KDP metadata, launch, ads, author funnel |
| compliance-reviewer | `../compliance-reviewer.md` | RESPA/TCPA/CAN-SPAM/FTC/platform risk check |

The agent files live directly in `.claude/agents/` so Claude Code loads them automatically in this repo. Run `/agents` to confirm.

## Use in other projects

```bash
cp .claude/agents/{growth-orchestrator,seo-strategist,content-optimizer,cro-specialist,book-marketer,compliance-reviewer}.md ~/.claude/agents/
```

## First prompt

```
Use growth-orchestrator to plan 90 days of SEO and conversion growth to get MLOs onto a monthly subscription. Domain: <your domain>.
```

Workflow: orchestrator -> seo-strategist + cro-specialist (parallel baseline) -> content-optimizer (build) -> compliance-reviewer (gate) -> publish -> seo-strategist (IndexNow) -> orchestrator (KPI review).

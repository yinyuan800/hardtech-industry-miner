# Evaluation scorecard

Use this rubric when ranking hard-tech routes, papers, teams, labs, startups, or investable directions. Keep scores directional unless the evidence supports precision.

## 1. Stage and bottleneck score

| Dimension | 1 | 3 | 5 |
|---|---|---|---|
| Demand urgency | interesting but optional | painful for some customers | blocks adoption or margin now |
| Commercialization timing | too early or already commoditized | pilots and early paid use | early scaling with unresolved bottleneck |
| Budget clarity | no clear payer | possible innovation/project budget | named buyer and budget line |
| Bottleneck durability | likely solved by baseline progress | may persist 12-24 months | structural bottleneck across many players |

## 2. Technical moat score

| Dimension | What to test |
|---|---|
| Scientific novelty | Is there a non-obvious mechanism or just engineering tuning? |
| Engineering depth | Does it require kernel, systems, hardware, data, process, or deployment know-how? |
| Replication time | How long would a strong incumbent need to match it? |
| Data/process advantage | Is there proprietary data, real-world feedback, manufacturing recipe, or customer workflow data? |
| IP/control | Are patents, trade secrets, licenses, or university-transfer rights defensible? |
| Benchmark credibility | Are tests realistic, current, reproducible, and compared to strong baselines? |
| Integration difficulty | Is deep integration required, and does that help or hurt commercialization? |

Score each 1-5, then classify:

- **Low moat:** mostly prompt/UI/packaging; easy to copy in weeks.
- **Medium moat:** useful algorithm/module; can be copied, but integration and tuning take quarters.
- **High moat:** system-level advantage with proprietary data/process/kernel/customer integration; replication takes 12+ months.
- **Very high moat:** architecture, hardware/process, regulatory, or data feedback loop creates compounding advantage.

## 3. Commercialization score

| Dimension | 1 | 3 | 5 |
|---|---|---|---|
| Customer pain | nice-to-have | department-level pain | executive-level cost/revenue blocker |
| Buyer access | unclear buyer | buyer exists but sales cycle long | clear buyer with urgent KPI |
| ROI measurability | hard to quantify | measurable in pilots | direct cost/revenue/SLA metric |
| Deployment friction | heavy migration, weak trust | integration needed but feasible | low-friction or mission-critical integration |
| Repeatability | bespoke project | repeatable with adapters | standardized product/license |
| Pricing power | weak, replaceable | module pricing | value-based pricing or savings share |

## 4. Startup-fit score

| Question | Strong signal | Weak signal |
|---|---|---|
| Is it a company or a feature? | expands into platform/workflow/system | single optimization easily absorbed |
| Can it wedge into customers? | solves urgent pain without replacing entire stack | requires full-stack replacement immediately |
| Can it survive big-company copying? | customers need neutrality, deployment, customization, or cross-platform support | only improves a model owned by one incumbent |
| Does it compound? | data, integrations, benchmarks, and deployment experience accumulate | each project restarts from zero |
| Can it get early revenue? | paid POC, license, deployment, or savings-share path | only future platform vision |

Classify:

- **Follow now:** technical and commercial scores high; next step is named-team/company diligence.
- **Watch:** technical signal strong but customer/ROI unproven.
- **Use as component:** useful module, weak standalone company.
- **Avoid:** weak moat, unclear buyer, or incumbent-copy risk dominates.

## 5. Technology-to-economics translation prompts

For every claimed technical gain, answer:

1. What exact metric improved? Under what hardware, dataset, baseline, and workload?
2. Which customer KPI changes: cost, latency, yield, throughput, quality, compliance, revenue, or risk?
3. What is the likely economic magnitude in a real deployment?
4. What adoption friction reduces the paper/demo gain?
5. Who pays, from what budget, and why now?
6. What would falsify the ROI claim?

## 6. Red flags

- Benchmark against weak or outdated baselines.
- No ablation, no failure cases, or no hardware/test setting.
- Speedup without quality, memory, or end-to-end serving measurement.
- “Commercial cooperation” described without named customer, scope, or repeat order.
- University IP ownership unclear for a proposed startup.
- Open-source code proves usefulness but removes scarcity.
- Customer must expose core model/data but has no reason to trust a startup.

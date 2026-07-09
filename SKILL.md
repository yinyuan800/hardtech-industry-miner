---
name: hardtech-industry-miner
description: "Use for hard-tech industry opportunity mining: start from a broad emerging industry trend, judge commercialization stage, map the value chain, identify technical bottlenecks, build a technology-route tree, scan papers/patents/open-source projects/research teams, translate technical metrics into customer economics, and produce an investable shortlist. Trigger when the user asks to 挖掘行业, 产业挖掘, 硬科技方向, 从大方向收敛到具体技术, 从论文/科研团队找商业化机会, 判断颠覆性技术, or identify hard-tech investment opportunities in AI, robotics, semiconductors, new energy, biotech, advanced manufacturing, or similar sectors."
---

# Hardtech Industry Miner

## Purpose

Use this skill to move from a broad industry signal to concrete hard-tech opportunities. The default output language is Chinese unless the user requests otherwise.

The core motion is:

`大趋势 -> 商业化阶段 -> 产业链/价值池 -> 核心瓶颈 -> 技术路线树 -> 论文/团队雷达 -> 技术经济翻译 -> 护城河/创业可行性 -> 可跟进机会清单`

Do not stop at market descriptions. End with specific directions, teams, papers, companies, validation questions, and what evidence would make the opportunity worth deeper diligence.

## Operating stance

- Treat the task as early-stage hard-tech opportunity discovery, not a conventional company profile.
- Prefer current primary sources: official model pages, papers, GitHub repos, patents, filings, lab pages, procurement records, cloud/API docs, benchmark reports, and named customer evidence.
- Browse when the topic depends on current industry status, model releases, funding, open-source activity, policy, pricing, or team information.
- Separate `[事实]`, `[公司口径]`, `[计算]`, and `[判断]` when the answer supports an investment or commercialization decision.
- Never equate hype, TAM, demo quality, paper benchmark, or announced partnership with obtainable revenue.
- Translate technical advantage through this chain: `measured performance -> customer consequence -> economic consequence -> durability`.
- If sources are missing, say what is unknown and lower confidence instead of filling gaps.

## Default workflow

### 1. Capture the trend trigger

Start by stating why this industry is worth looking at now:

- user/customer adoption inflection;
- technology breakthrough;
- cost curve decline;
- policy or localization driver;
- large-platform market education;
- supply-chain or regulatory shock;
- new open-source baseline that lowers entry cost.

Separate durable demand from short-term attention.

### 2. Judge commercialization stage

Classify the sector as one of:

| Stage | Evidence to look for | Opportunity implication |
|---|---|---|
| Research phase | mostly papers, weak demos, no repeat customers | watch technical teams and patents |
| Demo phase | impressive demos, limited production use | look for infrastructure and control bottlenecks |
| Early commercialization | first paid pilots, high cost, unstable workflows | best stage for hard-tech mining |
| Scaling phase | repeat contracts, platforms, standards forming | look for tools, picks-and-shovels, vertical winners |
| Red-ocean phase | commoditized products, price competition | avoid unless a deep bottleneck remains |

Explain the stage and the evidence behind it.

### 3. Map value chain and profit pools

Build the industry map before naming winners:

- upstream: data, chips, sensors, materials, compute, instruments, foundational IP;
- midstream: models, algorithms, systems, manufacturing/process, deployment stack;
- downstream: workflows, applications, channels, customers, compliance;
- adjacent infrastructure: security, evaluation, monitoring, simulation, standards.

Identify who pays, what budget line pays, what cost is reduced, and where gross margin could accrue.

### 4. Identify bottlenecks

Find 3-7 bottlenecks that block adoption or margin. Use concrete wording:

- too expensive;
- too slow;
- unstable quality;
- low yield;
- hard to control;
- hard to deploy on target hardware;
- lack of trusted data;
- missing certification/regulatory path;
- weak reliability or safety;
- integration friction with customer workflow.

Rank bottlenecks by: customer pain, technical difficulty, willingness to pay, and likelihood of remaining unresolved by incumbents.

### 5. Build the technology-route tree

For each bottleneck, map competing routes:

`bottleneck -> technical families -> representative papers/patents/repos/products -> expected customer/economic effect`

Use a tree or table. Include substitutes and incumbent in-house alternatives.

### 6. Scan papers, teams, patents, open source, and companies

For each promising route, look for:

- representative papers and benchmark claims;
- code availability, license, repo activity, stars/forks only as weak signals;
- continuity of output from the same lab/team;
- named professors, labs, alumni, startups, and industrial collaborators;
- patents or technology-transfer evidence;
- enterprise cooperation, procurement, pilots, or deployments;
- whether IP is likely owned by a university, company, or individual contributors.

When analyzing a paper, extract:

- problem solved;
- method in plain language;
- baseline and benchmark;
- exact performance improvement;
- hardware/test setting;
- failure cases and limitations;
- whether the method is training-free, retraining-heavy, data-heavy, or hardware-dependent;
- integration difficulty;
- whether a strong incumbent could reproduce it.

### 7. Translate technical metrics into economics

Convert technical results into business consequences:

- speedup -> GPU-hour cost, latency, throughput, concurrency, user wait time;
- memory reduction -> batch size, hardware tier, deployment density, edge feasibility;
- quality improvement -> retry rate, usable output ratio, customer conversion, SLA;
- yield/reliability -> scrap rate, warranty, certification, gross margin;
- control/safety -> enterprise adoption, compliance, repeatability;
- localization/hardware fit -> procurement eligibility and deployment budget.

Show formulas or ranges when possible. If a paper only reports benchmark scores, state why ROI cannot yet be estimated.

### 8. Score moat and startup fit

Use the scorecard in `references/evaluation-scorecard.md` when the user asks for ranking, investment judgment, or which direction is best.

Always distinguish:

- good paper vs good product;
- useful module vs standalone company;
- project-service business vs scalable software/IP business;
- big-company feature vs startup wedge;
- near-term revenue vs long-term platform potential.

### 9. Produce the opportunity map

End with a concise shortlist:

- 3-5 most promising hard-tech directions;
- representative papers/teams/companies;
- why now;
- customer and buyer;
- business model;
- moat depth;
- main risk;
- next evidence to verify;
- follow / wait / avoid recommendation.

If the user wants a deeper deliverable, use `references/output-templates.md` for report structure.

## Output modes

Choose the smallest output that satisfies the request:

- **Quick take:** 5-10 bullet conclusions and a ranking table.
- **Research note:** summary, viewpoints, technology tree, shortlist, open questions, sources.
- **Investment map:** full funnel, scoring matrix, named teams, business models, diligence checklist.
- **Paper/team diligence:** apply the workflow to one paper, lab, or startup and end with commercialization judgment.

## Hard filters

Flag or downgrade opportunities when:

- the advantage is only a UI/workflow wrapper and the user asked for hard tech;
- no customer has a budget line or urgent pain;
- performance gains appear only in toy benchmarks;
- the system requires access that customers will not provide;
- the technology is easy for a large model/platform company to copy;
- the business is mostly bespoke services without a path to repeatability;
- regulatory/IP ownership is unclear and material;
- open-source baselines already remove the scarcity of the claimed capability.

## Reference files

- Read `references/evaluation-scorecard.md` when ranking technologies, teams, commercialization potential, moat, or investment attractiveness.
- Read `references/output-templates.md` when producing a structured research note, investment map, or paper/team diligence memo.

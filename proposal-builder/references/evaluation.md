# Opportunity evaluation

Score only from supplied evidence. Use the weights as a decision aid, not false precision.

| Factor | Weight | What to assess |
| --- | ---: | --- |
| Required skills and deliverables | 30 | Direct or transferable ability to do the core work |
| Relevant evidence | 25 | Portfolio, outcomes, or experience pertinent to the request |
| Scope and feasibility | 20 | Clarity, timeline, access, dependencies, and ability to deliver |
| Budget and commercial fit | 15 | Known budget or rate relative to the work; unknown is not automatically bad |
| Client and platform risk | 10 | Policy issues, unpaid work, external payment, suspicious access, or contradictory terms |

For each factor, assign an anchored share of its weight:

- 100%: direct, sufficient evidence and no material unresolved issue.
- 75%: strong fit with one limited, resolvable uncertainty.
- 50%: transferable fit or a material unknown that requires clarification.
- 25%: weak evidence, several significant unknowns, or substantial remediation needed.
- 0%: no supporting evidence, clear incompatibility, or an unresolved blocker in that factor.

For client and platform risk, award more points when risk is low: 10 means no material warning signs, 5 means a resolvable warning, and 0 means an unsafe or prohibited condition. For budget, an unknown budget normally supports no more than half the available points unless other supplied commercial terms establish fit.

Verdicts:

- `APPLY`: 75-100 and no unresolved blocker.
- `APPLY WITH CONDITIONS`: 55-74, or a strong match with a material question that must be resolved before commitment.
- `SKIP`: below 55 or any blocker that makes the opportunity unsafe, misleading, or infeasible.

Explain the two or three factors that actually drive the verdict. A score must not override a hard blocker. When the job post or freelancer evidence is incomplete, show the uncertainty instead of awarding assumed points.

A prohibited or unsafe request is not automatically a permanent rejection of the entire opportunity. Treat it as resolvable only when the freelancer can explicitly decline that condition, remain within the platform, and offer a compliant alternative without exposing data, doing unpaid production work, or making an unsupported commitment. Use `APPLY WITH CONDITIONS` only when the rest of the opportunity remains a strong fit. Use `SKIP` when the client makes the condition mandatory, several warning signs combine, or proceeding would require unsafe access, policy circumvention, deception, or uncompensated project work.


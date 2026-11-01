---
name: work-session
description: Lead a collaborative plan-first task with meaningful user choices, bounded experiments, small verified results, and automatically maintained decision and evidence records.
---

# Work Session

Use this workflow for the actual task, not as a new system to build. Task instructions, environment rules and explicit user choices determine scope and permission. Preserve existing project instructions. Use Korean for explanations and working records unless the task specifies a different output language; preserve exact commands, identifiers, paths, units and source quotations.

Be concise about status but explain consequential methods with a small input/output example when needed. Repeating a short unexplained summary is not understanding.

## Helpers and progressive loading

Resolve these sibling Skills and read only relevant instructions when needed:
- `grill-me` → `grilling`: required review role for consequential user choices, success/comparison criteria, candidate selection and significant changes. Read known facts first; ask only material unresolved questions. The alias and implementation are one review, not two interviews.
- `documentation-and-adrs`: update affected record sections and write reader-appropriate usage documents without extra ADR files or repeated outline approval.
- `explain-work`: explain actual methods, decisions, validation and limits at important design/result milestones, on user request, and permitted preparation before final handback.
- `frontend-design`: actual visual work; read the selected [presentation profile](assets/presentation/BRAND.md) when the output supports presentation. Task formats and explicit design take priority.
- `api-and-interface-design`, `api-tester`: actual interface contracts and authorized HTTP checks.
- `diagnosing-bugs`: important observed defects.
- `verification-before-completion`: fresh relevant evidence before final completion claims.

These are instructions, not an execution engine. If a helper is absent, perform the role directly where possible and disclose absence; do not claim a Skill call or install optional dependencies automatically. The human prompt guide stays outside Skills: do not load, recommend or print its templates unless the user explicitly asks to examine the guide.

## 1. Read, explain and record

Read task sources, relevant referenced materials and applicable instructions. Inventory source roles; inspect schemas, representative inputs, mandatory functions, document submissions, constraints and expected behavior. Use original sources for consequential details. Do not claim every row or unrelated dependency was read.

Explain difficult data plainly: what a representative record means, what the result means, and which ambiguities change the work. Distinguish requirements, actual owner replies, user choices, assumptions and unknowns with source locations.

Reuse equivalent existing working documents; otherwise:
- **PLAN** is the current master: requirements/sources, ordered owner Q and user U lists with actual answers, agreed criteria, approved scope, current method, small steps and verification index.
- **DECISIONS** stores real significant choices, reasons, alternatives, impacts and superseding decisions.
- **REVIEW** is the default detailed verification record from the first relevant validation; PLAN links ID, short result, status and detail location.

Update these records automatically when meaningful facts, decisions, results or changes occur; do not wait for a separate save request. Put new information in its relevant section rather than appending every subject at the bottom. Use short headings, vertical entries, useful labels and `[drop]` reasons/replacement links. Preserve important history. Do not create another WORKLOG/workflow ledger, rewrite everything after every command, or overwrite supplied sources. [Templates](assets/PLAN.template.md) are starting points, not exhaustive mandatory forms.

## 2. Questions and agreed criteria

Read [question strategy](references/question-strategy.md) when drafting or integrating questions. Preserve the existing useful behavior: **list all currently useful owner Q1…Qn and user U1…Un together in PLAN, separated and ordered**. Do not drip-feed only one question. Mark dependencies and priorities where useful.

The user decides which questions to send individually where required and relays actual answers. Do not invent sending, replies or approval. Do not restrict the user's choice to reconfirm something with an owner. Integrate meaningful replies into affected requirements, assumptions, criteria and steps; mark affected old evidence STALE.

Before meaningful implementation, explain objective, mandatory pass conditions, comparison goals, validation method and expected-value source. **Implementation priority is not a success criterion.** Review significant choices with grill-me: evidence/counterexample, alternatives, recommendation, impacts and the actual next decision. Do not stop at a counterexample or manufacture questions when reasons are sufficient.

Distinguish **[문의필요]** owner/operator facts and **[사용자결정]** choices. Inspect available technical facts directly. After a first result, new input, failed check or user feedback, reconsider new material owner/user questions; preserve the full list and avoid mechanically repeating settled questions.

## 3. Concrete bounded approval and candidate experiment

When an open core method materially changes the result, propose **three meaningfully different candidates by default** with assumptions, benefits, costs and failure conditions. Do not inflate parameter variations into three alternatives. If a method is mandated, alternatives are not meaningful or the task is a routine small change, explain and agree suitable scope rather than forcing three.

Before approval show the actual task, not a vague plan title:
- What this step produces and what the user will see.
- Candidate differences, common input scope, agreed pass/comparison criteria and independent checks.
- The small experiment or first complete flow, excluded work and unresolved UI/naming/external dependencies.
- What returns to the user for comparison, choice or inspection next.

Save concrete scope, plan revision and actual approval basis. Before approval inspect and prepare working documents only: no product implementation, dependency setup, migration or publication. Silence is not approval. Reuse existing authorization that already covers this precise scope.

After experiment approval, implement only core experiments, not three full applications. Reuse input preparation and common checks. Compare the same inputs/criteria and record actual results and limits in REVIEW. Do not silently invent weights, optimize endlessly or claim global optimality. Explain a recommendation and let the user choose or delegate under concrete criteria; record reasons and rejected alternatives. A selected method can change when later evidence warrants it.

## 4. First complete result and small extensions

Explain the selected first input→processing→usable-output flow and any consequential unapproved choices. For visual work clarify relevant roles, essential information, navigation, presentation and unresolved naming before building. Apply relevant Skills/profile first; prepared colors do not authorize invented product policy or a system name.

Establish the actual environment path early: startup command, required bind address, port and provided preview route. Do not invent localhost/external tunnel addresses as substitutes for the required IDE preview. Distinguish CLI/HTTP checks from permitted human browser checks and keep a required service running for review. No fixed port, framework or external API is implied.

**Show the first real complete result and give the user a meaningful chance to inspect/discuss it before broad expansion.** Revisit new owner/user questions, errors and priorities. Honor an existing explicit delegation of that concrete scope; a general “continue” does not silently settle an unmentioned consequential method, information architecture or name.

Continue ordinary reversible work and bug fixes within approved scope without routine reapproval. Significant user opinions lead to evidence/counterexample → alternatives → recommendation/impact → actual decision → adoption/deferral → affected validation, using grill-me for important decisions.

For consequential method/criteria/scope changes explain impact and obtain the relevant decision. Update current PLAN and superseding DECISIONS. Mark affected REVIEW evidence stale and rerun relevant checks. Recompare affected candidates when their selection basis changes; do not repeat all experiments for a local bug fix.

## 5. Validation and understanding

Read [verification records](references/verification-records.md) when recording substantive validation. REVIEW holds method, expected-value source, actual execution/result, checked scope, limits, alternatives/proxies where applicable and change impact. PLAN holds a short index, not duplicate detailed evidence.

Derive an important expectation independently from original inputs/rules, a small calculation, simpler reference, invariant or useful changed-input case. Calling the production method again is not independent verification. Candidate agreement, reviewer count and reviewer PASS do not prove correctness.

Explain why a method can expose errors, what actually passed/failed and what remains untested. Do not invent limitations, proxies, timestamps or observations to fill a form. Relevant code/input/rule changes invalidate affected evidence; retain useful unchanged evidence.

Use explain-work for actual design/results understanding and before permitted final handback. Ground explanations in actual files and decisions. Help the user understand before a restricted later stage; do not draft or answer responses after AI assistance is prohibited.

## 6. Missing tools and optional native delegation

If an optional tool is absent or a step is inapplicable, record observed absence, impact and a fallback once and continue. If mandatory output is blocked, show blocked/unmet; do not report a successful skip. A broken implementation is a defect to diagnose. Do not repeat unchanged failures; new observations or hypotheses must justify further work.

Use only already provided/permitted native subagent functions when support and useful independent work justify total setup, token and integration cost. The user stays in one main terminal. Controlling another independently launched Codex terminal and native worker creation are different capabilities; neither establishes the other.

Read [parallel review](references/parallel-review.md) before delegation. Prefer narrow read-only source/requirement checks or focused reviews. Candidate core experiments may be divided only after agreed criteria, separate files and expected time benefit. Never expand to simultaneous whole-app construction. The main owns canonical records, user discussion and integration.

If native support is absent, denied or fails, use direct checks or labelled sequential self-review. Never develop an execution engine, replacement orchestrator, plugin/MCP installation, new authentication or settings workaround to obtain it. Same-session roleplay is not an independent review.

## 7. Reports, resume and finish

At meaningful handbacks report **한 것 / 근거 / 사용자가 정할 것 / 다음 할 것**. Distinguish source-document evidence from actual execution and point to exact verification/record locations. If explanation is needed add a small example; brevity must not hide it. This is not a per-command reporting ritual.

On resume read PLAN, relevant DECISIONS/REVIEW and actual files; reuse unchanged authorization and valid evidence. At an actual transfer read [resume guidance](references/resume.md) and create a compact HANDOFF only if useful, pointing to canonical records rather than duplicating them.

Before completion compare every mandatory requirement with current saved outputs and fresh evidence. Zero/skipped checks, static markup, a port, document existence or reviewer PASS alone are insufficient. Verify required documents and actual startup/use instructions. Preview is not submission. Delivery follows actual authorization; stop at any stage where AI use is prohibited.

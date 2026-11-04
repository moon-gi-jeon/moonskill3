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
- `explain-work`: maintain the participant's actual-work understanding document at important design/result milestones and before permitted final handback. Read its outline when first needed; do not wait for the participant to remember another Skill name.
- `frontend-design`: actual visual work; read the selected [presentation profile](assets/presentation/BRAND.md) when the output supports presentation. Task formats and explicit design take priority.
- `api-and-interface-design`: read before designing an actual API contract, including an internal endpoint used by the app. `api-tester`: read before the first authorized HTTP check of an actual API. Apply only the relevant part and record the contract or check, or why the helper was unavailable or inapplicable.
- `diagnosing-bugs`: important observed defects.
- `verification-before-completion`: fresh relevant evidence before final completion claims.

These are instructions, not an execution engine. If a helper is absent, perform the role directly where possible and disclose absence; do not claim a Skill call or install optional dependencies automatically. The human prompt guide stays outside Skills: do not load, recommend or print its templates unless the user explicitly asks to examine the guide.

The model selects relevant helpers; the participant need not invoke each one at every stage. For substantive calculations use [test reasoning](references/test-reasoning.md); diagnosing-bugs is for an observed defect, not the default name for all algorithm validation. At a meaningful handback identify a newly applied helper and its purpose briefly, or link the relevant PLAN entry. Distinguish installed/discovered, instruction read or already in context, actual role performed, unavailable and not applicable. Do not claim a hidden automatic engine or independent reviewer.

## 1. Read, explain and record

Read task sources, relevant referenced materials and applicable instructions. Inventory source roles; inspect schemas, representative inputs, mandatory functions, document submissions, constraints and expected behavior. Use original sources for consequential details. Do not claim every row or unrelated dependency was read.

Explain difficult data plainly: what a representative record means, what the result means, and which ambiguities change the work. Distinguish requirements, actual owner replies, user choices, assumptions and unknowns with source locations.

Reuse equivalent existing working documents; otherwise:
- **PLAN** is the current master: requirements/sources, ordered owner Q and user U lists with actual answers, agreed criteria, approved scope, current method, small steps and verification index.
- **DECISIONS** stores real significant choices, reasons, alternatives, impacts and superseding decisions.
- **REVIEW** is the default detailed verification record from the first relevant validation; PLAN links ID, short result, status and detail location.

Update these records automatically when meaningful facts, decisions, results or changes occur; do not wait for a separate save request. Put new information in its relevant section rather than appending every subject at the bottom. Use short headings, vertical entries, useful labels and `[drop]` reasons/replacement links. Preserve important history. Do not create another WORKLOG/workflow ledger, rewrite everything after every command, or overwrite supplied sources. [Templates](assets/PLAN.template.md) are starting points, not exhaustive mandatory forms.

Use the [record layout](references/record-layout.md) to make mandatory conditions, constraints, required functions/documents and the next user choice easy to find without duplicating their full definitions. The local review layout uses bracketed headings. Preserve equivalent existing records and meaningful history. In the initial PLAN, put the whole provisional S-ID sequence just below current status as short task-specific outcomes. Use the same IDs in current status and stage reports. Initial source interpretation and useful questions deserve adequate time; do not rush them to satisfy an invented universal timer or change model effort to repair an unmeasured bottleneck.

At the top of each task document created or maintained, briefly identify its role, authoritative content and where related decisions, verification or explanations actually live. Use the actual filenames/IDs and distinguish planned documents from existing ones. Required task formats take priority; do not edit supplied sources or create empty files just to complete this map. Follow the record layout for the four document roles and conditional handoff/use documents.

Save a new decision or verification detail before linking it as completed from PLAN. Do not point to an unsaved planned ID as if evidence exists. On interruption/resume check relevant new links and current versus historical status; disclose gaps rather than reconstructing unwritten past facts.

## 2. Questions and agreed criteria

Read [question strategy](references/question-strategy.md) when drafting or integrating questions. Preserve the existing useful behavior: **list all currently useful owner Q1…Qn and user U1…Un together in PLAN, separated and ordered**. Do not drip-feed only one question. Mark dependencies and priorities where useful.

The user decides which questions to send individually where required and relays actual answers. Do not invent sending, replies or approval. Do not restrict the user's choice to reconfirm something with an owner. Integrate meaningful replies into affected requirements, assumptions, criteria and steps; mark affected old evidence STALE.

For each unresolved user choice provide options, a recommendation with reasons/counterexample and material impact, the actual requested decision, and a waiting/selected/delegated status. If evidence is insufficient, explain why the recommendation is provisional or withheld. After an actual reply update that same U entry, the selection and affected records automatically. Never fabricate retrospective recommendations or turn the model's recommendation into approval.

Before meaningful implementation, explain objective, mandatory pass conditions, comparison goals, validation method and expected-value source. **Implementation priority is not a success criterion.** Review significant choices with grill-me: evidence/counterexample, alternatives, recommendation, impacts and the actual next decision. Do not stop at a counterexample or manufacture questions when reasons are sufficient.

Distinguish **[문의필요]** owner/operator facts and **[사용자결정]** choices. Inspect available technical facts directly. After a first result, new input, failed check or user feedback, reconsider new material owner/user questions; preserve the full list and avoid mechanically repeating settled questions.

## 3. Concrete bounded approval and candidate experiment

When an open core method materially changes the result, consider **three meaningfully different feasible candidates by default under the same complete mandatory requirements**. Each candidate must preserve those requirements; an option that deliberately drops one is not a qualifying candidate. Show assumptions, benefits, costs, failure conditions and the evidence still needed to establish feasibility. A proposal is not yet a verified result. Do not inflate parameter variations or fill a third slot for appearances. If time, evidence or clear dominance makes two or fewer meaningful candidates appropriate, explain the actual comparison scope and proceed with the supported set rather than wasting time to reach three.

For constrained selection, allocation or other consequential methods read [method selection](references/method-selection.md). Include the required guarantee, implementation/integration/validation/explanation cost, remaining permitted time and a fallback trigger. Validate the qualifying candidates' actual results against the same mandatory conditions before ranking them. Preserve comparable numerical results and the rationale for the selected best/optimal candidate within the agreed scope; do not imply an unproved global guarantee. Estimates stay estimates and are updated from observations. Time pressure can reduce the number of candidates, not silently weaken a mandatory requirement.

This comparison is a pre-implementation safeguard: explore different possibilities, substantiate the choice and reduce avoidable late core redesign. Preserve the quantitative rationale so the participant understands the decision. It is not a ban on later correction when new evidence justifies changing the method.

Before approval show the actual task, not a vague plan title:
- What this step produces and what the user will see.
- Candidate differences, common input scope, agreed pass/comparison criteria and independent checks.
- The small experiment or first complete flow, excluded work and unresolved UI/naming/external dependencies.
- What returns to the user for comparison, choice or inspection next.

For a consequential approval explanation, recommend a concrete task-specific option with its reasons, material counterexample/condition, tradeoff and effect on this scope. Existing U recommendations apply to criteria, candidate experiments, first implementation and significant UI/method changes, not only to an initial interview. If evidence is insufficient, explain a conditional recommendation or why it is withheld; do not invent an option, number or decision. This clarifies existing approval points and does not add approval of routine work.

When a CLI cannot show the full explanation use PLAN as its readable location, in the relevant U/step section. Reuse that U/S-ID where sufficient; use a stable X01-style explanation ID only if needed, not another document or ledger. Keep the immediate decision, recommendation, principal reason, consequential condition/risk and approval scope visible in the terminal, and point to the exact PLAN ID for detail. A path or vague title alone is not an approval explanation. Record the actual reply and approved revision against that explanation; a recommendation or an unanswered document is not approval.

Save concrete scope, plan revision and actual approval basis. Before approval inspect and prepare working documents only: no product implementation, dependency setup, migration or publication. Silence is not approval. Reuse existing authorization that already covers this precise scope.

After experiment approval, implement only the necessary core experiments, not multiple full applications. Reuse input preparation and common checks. Check feasibility first, then compare qualifying results on the same inputs/criteria. Record measured values, units, input scope, relevant differences, expected-value sources and limits in REVIEW. Nonqualifying results may explain a rejection but do not fill the feasible-candidate count. Do not silently invent weights, optimize endlessly or claim global optimality. Explain a recommendation and let the user choose or delegate under concrete criteria; record numerical reasons and rejected alternatives. A selected method can change when later evidence warrants it.

## 4. First complete result and small extensions

Explain the selected first input→processing→usable-output flow and any consequential unapproved choices. For visual work clarify relevant roles, essential information, navigation, presentation and unresolved naming before building. Apply relevant Skills/profile first; prepared colors do not authorize invented product policy or a system name.

Recommend a concrete initial information layout and applicable prepared profile when the actual task supports them: explain which information/actions belong in the primary view, which are secondary, and why this serves the roles and required flow. Make provisional choices and exclusions clear. Prepared assets support the recommendation; they do not authorize a fixed dashboard, invented name or new feature. Keep long rationale under the approval explanation's PLAN ID.

Before the first web implementation, record the start command, bind address and port required by the task, and the IDE-provided fixed or generated preview URL when available. If a required detail is visible only to the user or cannot be verified, ask for that detail or mark the preview blocked; never guess the URL or port. Run the app in the task workspace and use the provided IDE preview when required. Do not use public hosting, external deployment, or tunnels as substitutes. Keep the service available for the user's first-result check and record server/HTTP evidence separately from the user's actual IDE browser observation.

**Show the first real complete result and give the user a meaningful chance to inspect/discuss it before broad expansion.** For a UI, give the user role → input or action → expected screen in the actual IDE preview. During final checks group manual actions still unverified or affected by changes. Revisit new owner/user questions, errors and priorities. Honor an existing explicit delegation of that concrete scope; a general “continue” does not silently settle an unmentioned consequential method, information architecture or name.

Continue ordinary reversible work and bug fixes within approved scope without routine reapproval. Significant user opinions lead to evidence/counterexample → alternatives → recommendation/impact → actual decision → adoption/deferral → affected validation, using grill-me for important decisions.

For consequential method/criteria/scope changes explain impact and obtain the relevant decision. Update current PLAN and superseding DECISIONS. Mark affected REVIEW evidence stale and rerun relevant checks. Recompare affected candidates when their selection basis changes; do not repeat all experiments for a local bug fix.

## 5. Validation and understanding

Read [verification records](references/verification-records.md) when recording substantive validation. REVIEW holds method, expected-value source, actual execution/result, checked scope, limits, alternatives/proxies where applicable and change impact. PLAN holds a short index, not duplicate detailed evidence.

Derive an important expectation independently from original inputs/rules, a small calculation, simpler reference, invariant or useful changed-input case. Calling the production method again is not independent verification. Candidate agreement, reviewer count and reviewer PASS do not prove correctness.

Explain why a method can expose errors, what actually passed/failed and what remains untested. Do not invent limitations, proxies, timestamps or observations to fill a form. Relevant code/input/rule changes invalidate affected evidence; retain useful unchanged evidence.

REVIEW starts with short current checks grouped by what they mean to the user: why the check matters, how it works, why the expected result is credible, actual result, limitation and the detailed V-ID. Keep execution history and full evidence below. Readable explanations supplement the evidence; they do not replace it or justify extra reruns merely because prose changed.

Use explain-work for actual design/results understanding and before permitted final handback. Ground explanations in actual files and decisions. Help the user understand before a restricted later stage; do not draft or answer responses after AI assistance is prohibited.

Maintain one actual-work understanding document, normally PROJECT_GUIDE.md or an existing equivalent. Use the document title “프로젝트 결과와 의사결정 해설”. Reuse an existing equivalent, including legacy UNDERSTANDING.md, rather than creating a duplicate or renaming already-linked task records; mandated task names and formats take priority. It explains purpose/scenarios, core method and alternatives, key verification reasoning, important process changes, difficult/boundary cases, limitations/proxies, actual user/AI contributions and the assignment's real collaboration questions. Preserve detailed explanations and present the topic-by-topic recap followed by six distinct predicted practice questions and evidence-based answer cues at the top. Describe actual work and decision changes in chronological order. Use explain-work to reconcile this top section with the saved result during the permitted final handback. Update affected sections after important decisions/results and reconcile it before permitted final handback; do not create a second understanding ledger or invent missing events. Required output names and file whitelists take priority.

## 6. Missing tools and optional native delegation

If an optional tool is absent or a step is inapplicable, record observed absence, impact and a fallback once and continue. If mandatory output is blocked, show blocked/unmet; do not report a successful skip. A broken implementation is a defect to diagnose. Do not repeat unchanged failures; new observations or hypotheses must justify further work.

Use only already provided/permitted native subagent functions when support and useful independent work justify total setup, token and integration cost. The main terminal owns implementation and final verification. A permitted second terminal is an optional read-only independent review route. Controlling another independently launched Codex terminal and native worker creation are different capabilities; neither establishes the other.

At the first handback after saving and verifying a consequential result, consult [parallel review](references/parallel-review.md) to decide whether to recommend independent review and prepare the request. Use the same reference before any delegation. On the user’s request, read the selected findings in INDEPENDENT_REVIEW.md, reproduce them against current saved artifacts and record the disposition in REVIEW. Prefer narrow read-only source/requirement checks or focused reviews. Candidate core experiments may be divided only after agreed criteria, separate files and expected time benefit. Never expand to simultaneous whole-app construction. The main owns canonical records, user discussion and integration.

If native support is absent, denied or fails, use direct checks or labelled sequential self-review. Never develop an execution engine, replacement orchestrator, plugin/MCP installation, new authentication or settings workaround to obtain it. Same-session roleplay is not an independent review.

## 7. Reports, resume and finish

At the end of initial planning, a candidate experiment, a first result, a consequential change or final validation, use the four visible labels **한 것 / 근거 / 사용자가 정할 것 / 다음 할 것**. If no decision is pending, write `없음` in that line. Distinguish source-document evidence from actual execution and point to exact verification/record locations. If explanation is needed add a small example; brevity must not hide it. After those four lines, add one short PLAN-based line when there is a relevant step: [현재 S-ID · 단계명 · 실제 상태] → [다음 S-ID · 결과/행동]. Omit an inapplicable next step and name a real blocker rather than inventing one. For consequential blockers, identify the held step and U-ID, already authorized independent work if any, and one immediate action. This is not a per-command reporting ritual.

For a pending consequential choice include the recommendation and exact explanation ID, not only a request to read PLAN. For a factual result or observation request, give the relevant finding/check and next action without manufacturing alternatives. Document role headers and PLAN's live links should let any reader find the detailed V-ID in REVIEW, decision D-ID in DECISIONS, and accessible project explanation without guessing.

On resume read PLAN, relevant DECISIONS/REVIEW and actual files; reuse unchanged authorization and valid evidence. At an actual transfer read [resume guidance](references/resume.md) and create a compact HANDOFF only if useful, pointing to canonical records rather than duplicating them.

Before completion compare every mandatory requirement with current saved outputs and fresh evidence. Zero/skipped checks, static markup, a port, document existence or reviewer PASS alone are insufficient. Track each assignment-required document by its actual name, format and requirement ID in PLAN. When evidence is ready within approved work, use documentation-and-adrs to draft or update it from PLAN, DECISIONS, REVIEW and actual outputs. At final check or resume, distinguish the required path, current saved presence, content/format evidence and user/platform confirmation of actual submission under the existing requirement ID. Verify actual startup/use instructions where required. Preview is not submission. Delivery follows actual authorization; stop at any stage where AI use is prohibited.

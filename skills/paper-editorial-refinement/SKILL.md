---
name: paper-editorial-refinement
description: "Refine existing manuscript information organization and expression while preserving scientific meaning. Use to diagnose reading obstacles, propose edits, or revise connected prose, captions, equations, labels, and appendices. Choose editorial actions from the role of the information; submission-readiness verdicts are a separate task."
---

# Paper Editorial Refinement

Help a reader understand what was done, interpret the evidence, and locate supporting detail. Work from a supplied manuscript or excerpt and its relevant context. This skill supplies an editing decision method, not a prescribed paper structure or a style makeover. It works independently of any project, model, or companion skill.

## Establish the requested work

Distinguish **inspection**, **a proposed revision**, and **editing the manuscript** from the current request. Inspection or discussion does not authorize source edits. A proposal can include replacement wording in the response without changing files. Execute explicitly authorized revisions without asking for approval of every routine edit. Keep any scope boundaries the user supplied; flag necessary linked changes outside them rather than silently expanding the assignment.

Read the relevant passage and enough surrounding material to identify its purpose, definitions, evidence, and downstream uses. Use a current rendered page when the question concerns visual layout. With only an excerpt, give a local result and identify any dependencies you could not inspect; do not demand an entire manuscript for a small edit.

If author decisions are available, distinguish approved requirements, suggestions, rejected alternatives, and later changes of direction. Preserve the scope of an approval. Neither an assistant suggestion nor a locally preferred sentence establishes a manuscript-wide rule. Use aesthetic preferences only when explicitly supplied; do not infer a color palette or visual style from one accepted layout.

## Editorial decision method

Use this reasoning internally at the scale of the problem. A sentence edit need not produce a five-step report.

1. **Locate the reading obstacle.** State what the reader cannot determine at a specific location: the purpose of an operation, what a denominator counts, which label denotes the same method, why a comparison matters, or where needed evidence is found. Length, an abbreviation, or a short final line alone is not a demonstrated obstacle. If the passage already works, retain it.
2. **Identify the information's role.** Does it establish the question or design rationale, define an object, enable local interpretation, support a claim, or provide reproduction detail? An item can have more than one role. A threshold used in a protocol may also be essential for interpreting a column; do not move it merely because it is technical.
3. **Choose the smallest sufficient action.** Add a missing explanation supported by supplied material; rewrite an ambiguous relation; move a coherent unit to where it is needed; merge true repetition; or keep the original. Several actions can work together. Do not invent a design rationale, a definition, or a scientific premise to make prose flow.
4. **Apply connected changes.** Identify affected definitions, equation references, table or figure labels, captions, results discussion, and appendix pointers. Preserve meaning across those locations. Update the maintained source of generated text when it is within scope, not just the generated artifact. If that source is unavailable, report the remaining synchronization work. Do not regenerate experiments to change a label.
5. **Check whether the obstacle is resolved.** Re-read the result as a reader and compare it against the original scientific content. Check moved text at both origin and destination, its pointers, and any affected rendered pages. Stop when the targeted information is understandable and the linked content is consistent; another possible phrasing is not a reason to continue.

## Choose locations by reader need

| Information role | Placement decision |
| --- | --- |
| Question, design purpose, essential operation, decisive evidence | Keep enough in the main text for the argument to stand. Put purpose before dense operations when the reader otherwise cannot understand why they are needed. Do not add a new introduction to every paragraph. |
| Meaning of a table cell or visual encoding | Keep the necessary reading instructions in the header, caption, or nearby note: relevant baseline, units, direction, eligibility, denominator, grouping, symbols, and missing-value meaning. Include only what that display needs. |
| Meaning of an equation | Explain the calculation's purpose and objects near the equation. Define conditions, denominator, aggregation, units, and comparison direction at the point of need. Reuse a nearby clear definition rather than repeating it mechanically. |
| Full protocol, implementation detail, extended derivation | Place detailed material in a navigable appendix when a concise main-text description is enough to understand and assess the work. Retain locally necessary definitions and genuine interpretive limitations. |
| Supplementary result | Move its detailed claim together with the interpretation that depends on it; retain only conclusions supported by main-text evidence. Do not solve a display problem by removing numbers while retaining the unsupported inference. |

A caption should establish the display's purpose or a supported observation and make it readable. Its job is not to be as short as possible. Move a full procedure or repeated explanation out only when the remaining caption still identifies what the reader is comparing. Thresholds, group rules, and denominators sometimes belong locally even if also defined in Methods. Captions need not repeat every shared definition or follow a universal sentence order.

Substantive numerical results that remain in the main text should be displayed in its tables or figures, or be transparently derivable from compatible displayed values. Design counts, constants, and illustrative thresholds are not automatically result estimates. Relocation must not weaken that evidence connection. Do not reconstruct paired effects from rounded marginal summaries or silently change populations or aggregation to make values agree.

## Preserve meaning while refining expression

- **Methods and equations:** Make existing rationale and computation intelligible. Preserve mathematical conditions, signs, index sets, normalization, estimands, and units. A missing explanation is different from a wrong or underdetermined formula. Identify a contradiction at its affected locations and defer the dependent rewrite until the scientific choice is resolved; continue independent authorized edits. Do not use smoother wording to conceal an evidence or method conflict. Inline versus display math and line breaking depend on the expression and actual layout, not a one-equation-per-line rule.
- **Names and navigation:** Check that a definition, its table or figure label, and the discussion refer to the same object. Retain useful short labels once defined; distinguish an operation, a comparison, and an outcome when they are different objects. Do not perform a global replacement from a local naming choice. Preserve stable internal identifiers unless a change is necessary and authorized; repair affected references when text moves.
- **Defensive prose:** Merge repeated caveats and remove empty assurances or repeated justification that adds no information. Retain real uncertainty, negative findings, selection effects, and limits needed to interpret the claim where the reader needs them. A concise limitation is not permission to strengthen the conclusion, claim equivalence from similar estimates, or assert unverified guarantees.
- **Stage and scope:** During content work, fix reasoning, explanations, and information placement before compressing. During finishing, address authorized length and layout constraints without discarding essential evidence. Investigate the cause of whitespace or awkward wrapping before changing prose; do not stretch tables or add filler to occupy a page. Preserve clear passages and previously resolved choices unless relevant evidence or content changes.

## Check and deliver

Compare the affected material before and after for research facts, numerical values, formula meaning, claim strength, and material limitations. If information moves, check its new location and the claims remaining behind. Check terminology and references across the actual affected locations; report an inaccessible destination rather than asserting it is synchronized.

For visual claims or layout edits, inspect the actual current rendered output and the surrounding page. A source diff, text extraction, or successful build alone does not establish readability. Reuse the project's build process when available. If rendering or inspection is unavailable, complete the text work and mark visual verification as pending.

Match the delivery to the request:

- **Inspection:** Identify concrete obstacles, their locations, and suitable actions; say when keeping the original is justified.
- **Proposal:** Give replacement wording or a placement plan, necessary linked changes, and the conditions under which it works.
- **Revision:** Make the authorized edits, then summarize what changed, why, what was preserved, and what was checked. Include unresolved scientific choices or unavailable verification that materially limits the result.

For a small change, a brief explanation is enough. Do not produce scores, a readiness verdict, a mandatory change ledger, or a comprehensive paper review unless requested. The task is complete when the requested obstacles are resolved, linked changes within scope are consistent, and verification limits are explicit. If no material obstacle is found, keeping the original is a completed outcome.

## Examples and neighboring scope

Read [editorial cases](references/editorial-cases.md) when a concrete example helps choose among adding, rewriting, moving, merging, or retaining information. The five fictional cases include proposed results or a no-change response, with limits; they are not templates to impose on every paper or claims of measured improvement.

If available, `paper-submission-acceptance` supplies a readiness decision and its completion criteria, and can also help implement fixes. This module contributes the information-role and connected-edit decisions used to develop a revision, including work on an unfinished excerpt. Neither module requires running the other. Shared preservation and evidence constraints apply throughout; this module does not copy the readiness rubric or its report structure.

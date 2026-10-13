# Research Skills

[English](README.md) | [简体中文](README.zh-CN.md)

Practical skills for research and scientific writing. Each skill addresses a specific task, works on its own, and can fit into a larger research workflow. Skill instructions are written in English; you can request reports in your preferred language.

The current modules help researchers make submission-readiness decisions and refine the organization and expression of existing manuscripts.

## Available skills

| Skill | Use it when | What you get |
| --- | --- | --- |
| [Paper Submission Acceptance](skills/paper-submission-acceptance/SKILL.md) | You have a draft and need a submission-readiness decision, a focused revision plan, or a check of completed revisions. | A supported readiness judgment, substantive blockers, finishing work, unverified checks, and concrete completion conditions. |
| [Paper Editorial Refinement](skills/paper-editorial-refinement/SKILL.md) | A passage, caption, equation, or connected set of manuscript elements is hard to understand, and you want an inspection, proposal, or revision. | A concrete editorial choice based on the information's role, coordinated changes where authorized, and checks that meaning and references remain intact. |

## Paper Submission Acceptance

A manuscript can go through many revisions without a clear answer to “Is it ready?” Another review may add suggestions without explaining which ones matter or when revision can stop.

This skill assesses the research question, contribution, argument, evidence, readability, and final materials. It turns findings into decisions about what needs substantive work, what can enter finishing, and what is already sufficient.

Three practices guide the assessment:

- **Make main-text evidence checkable.** Substantive numerical results used in the main text belong in a main table or figure, or must be transparently derivable from displayed values. If a secondary numerical result moves to the appendix, its dependent detailed interpretation moves with it. Design counts, constants, and illustrative thresholds are not automatically result estimates.
- **Give issues completion conditions.** Each decision-relevant finding identifies a location, evidence, its effect on readiness, and what would resolve it. Missing material remains unverified rather than becoming an invented failure.
- **Let revision converge.** Preserve resolved decisions across passes. Reopen an issue for new evidence, a relevant manuscript change, or a contradiction. Local wording preferences need not restart substantive revision.

The report leads with one status:

| Status | Meaning |
| --- | --- |
| Substantive revision needed | A demonstrated issue prevents a central claim from being assessed or sustained. |
| Ready for finishing | The research and argument are stable; bounded presentation or package work remains. |
| Ready to submit | Substantive criteria and applicable final checks pass for the inspected version. |
| Readiness not fully verified | Missing materials or checks prevent a complete verdict. |

An assessment does not submit or edit your manuscript. It does not predict acceptance. When you also request fixes, the skill supports completing that authorized work.

## Local use and acceptance examples

Copy the complete directory of the skill you want from `skills/` into your agent's supported skill directory, or point your agent at that module's `SKILL.md`. Keep its bundled references with it. Neither module requires companion skills or scripts. Available file readers, PDF viewers, and search tools determine which checks can be completed; unavailable checks must be reported as unverified.

Provide the current manuscript, relevant figures and tables, and any appendix. For final checks, provide the rendered PDF and applicable submission requirements. Previous findings help when checking a revision. You can begin with incomplete materials and receive a scoped assessment.

Example requests:

- “Use paper-submission-acceptance to assess this manuscript. Separate substantive blockers from finishing work.”
- “Check whether substantive numbers discussed in the main text are supported by its tables and figures.”
- “Recheck the previous issues against this revision. Preserve resolved decisions unless the changes affect them.”
- “Can substantive revision stop? Explain what still prevents a readiness decision.”

Two fictional examples show the assessment in practice:

- [A result transparently derivable from the main table](examples/submission-readiness.md): distinguish wording fixes from unverified final checks.
- [Numerical evidence appears only in the appendix](examples/missing-main-text-evidence.md): identify an unmet display requirement and resolve it without inventing a need for new experiments.

These examples illustrate behavior, not measured performance.

## Paper Editorial Refinement

A technically correct manuscript can still make readers work unnecessarily: an equation's objects are defined too far away, a caption mixes reading instructions with a full protocol, or one method has different names in the definition and results.

This module turns those obstacles into editing decisions:

**Locate the obstacle → identify the information's role → choose an action → coordinate related edits → check the result.**

The available actions include adding a supported explanation, rewriting an ambiguous relation, moving information, merging repetition, and keeping the original. Information needed to understand or assess a result stays accessible; reproduction detail can move to an appendix when that does not weaken the main argument. Captions keep the thresholds, symbols, and denominators needed for their particular display. Revisions preserve facts, values, formula meaning, claim strength, and genuine limitations.

Provide the passage or manuscript, relevant definitions and displays, and whether you want inspection, proposed wording, or actual edits. Include a rendered page for layout questions and explicit style preferences if you have them. An excerpt is enough for a local task; inaccessible related material is reported as a coverage limit.

Example requests:

- “Use paper-editorial-refinement to inspect this caption. Which information should stay here, and which belongs in Methods or the appendix? Do not edit files.”
- “Propose an explanation for this formula using the supplied definitions. Preserve its denominator and comparison direction.”
- “Revise the method description, table labels, and results references so they identify the same procedure. Update the caption generator too.”
- “Remove repeated defensive language while retaining uncertainty, negative results, and the limits needed to interpret the findings.”
- “Check whether this paragraph actually needs revision. Keeping it unchanged is acceptable.”

The [five fictional editorial cases](skills/paper-editorial-refinement/references/editorial-cases.md) show inputs, obstacles, choices, proposed results, and limits, including a justified no-change outcome. They illustrate decisions, not measured effectiveness.

## Place in a larger workflow

Call **Paper Submission Acceptance** when the question is whether a manuscript is ready and what must be completed. Call **Paper Editorial Refinement** when the question is how to make specific information understandable and place it effectively, even in an unfinished excerpt. Acceptance can also help implement fixes; refinement adds the information-role and connected-edit method for developing those revisions. Neither module automatically runs the other.

Both preserve scientific meaning, evidence accessibility, scoped authorization, and honest verification. The detailed readiness rubric and verdicts remain in the acceptance module; editorial action selection and its cases live in refinement. Only the short preservation constraints needed for standalone use overlap. When changing an overlapping constraint, check both modules for consistency rather than copying their full workflows or adding a mandatory shared dependency.

Additional modules can be added under `skills/` as their tasks become concrete. Each module should state when to use it, what it produces, and how to tell when its work is complete.

## License

This repository's skills, documentation, and examples are released under the [MIT License](LICENSE).

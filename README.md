# Research Skills

[English](README.md) | [简体中文](README.zh-CN.md)

Practical skills for research and scientific writing. Each skill addresses a specific task, works on its own, and can fit into a larger research workflow. Skill instructions are written in English; you can request reports in your preferred language.

The first module helps researchers decide whether a manuscript is ready to submit and what still needs to change.

## Available skills

| Skill | Use it when | What you get |
| --- | --- | --- |
| [Paper Submission Acceptance](skills/paper-submission-acceptance/SKILL.md) | You have a draft and need a submission-readiness decision, a focused revision plan, or a check of completed revisions. | A supported readiness judgment, substantive blockers, finishing work, unverified checks, and concrete completion conditions. |

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

## Use locally

Copy the complete `skills/paper-submission-acceptance/` directory into your agent's supported skill directory, or point your agent at its `SKILL.md`. The skill requires no companion skills or scripts. Available file readers, PDF viewers, and search tools determine which checks can be completed; unavailable checks must be reported as unverified.

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

## Place in a larger workflow

Use this module after drafting or revision, whenever you need a readiness decision. It can work with writing, evidence-verification, and submission-package tools, without requiring a particular skill family or a fixed sequence of stages.

Additional modules can be added under `skills/` as their tasks become concrete. Each module should state when to use it, what it produces, and how to tell when its work is complete.

## License

This repository's skills, documentation, and examples are released under the [MIT License](LICENSE).

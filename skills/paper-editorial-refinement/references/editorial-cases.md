# Editorial decision cases

All five cases are fictional and use invented text and values. They illustrate editorial reasoning, not a real manuscript, a measured improvement, or an executed user study. The replacement text is a proposal unless the user has authorized editing. Each case supplies the scientific premises needed for its revision; do not invent equivalent premises in a real task.

## 1. A long caption contains both essential reading rules and a full procedure

**Input.** A table has rows Short and Long, and columns Positive / Eligible / Rate (%). The rows contain 18 / 30 / 60 and 15 / 30 / 50. Its caption reads:

> Positive rates by sequence length. Short sequences contain at most four observations; Long sequences contain more than four. Only sequences with every required observation enter the denominator. An eligible sequence is positive when its normalized score is at least 0.65. Records are first sorted by identifier, then normalized using the training-set mean and standard deviation, and evaluated with fixed preprocessing parameters. All parameters were selected using training data. We compare positive rates by sequence length.

Methods already describes the normalization and training-only parameter selection. Appendix B contains the preprocessing procedure but omits the record-sorting step.

**Reading obstacle.** The duplicated purpose and procedure obscure the rules needed to interpret the rows and percentages. Removing every technical detail would instead make the categories and denominator ambiguous.

**Information role and choice.** Keep grouping, positivity threshold, and denominator locally. Merge the repeated purpose. Retain the existing method definition; move the previously undocumented sorting step to the full procedure and add a useful pointer.

**Proposed result — caption:**

> Positive rates by sequence length. Short: at most four observations; Long: more than four. Positive means normalized score ≥ 0.65. Rates use only sequences with every required observation. Methods describes normalization and parameter selection; Appendix B gives the full preprocessing procedure.

**Linked appendix addition:**

> Records are sorted by identifier before normalization.

Integrate this wording with the existing Appendix B procedure rather than duplicating sentences already there. Keep table values and the existing normalization definition unchanged. If a generator owns the caption, edit its text source too within the authorized scope.

**Completion and boundary.** A reader can recover row membership, positivity, denominator, and procedure location. Check the caption on its rendered page before claiming it is visually improved. The threshold stays local because it defines the displayed outcome. If a threshold only controls an unrelated implementation detail, this case would not justify keeping it in every caption. No observed between-group difference is claimed to be causal or statistically established.

## 2. A correct formula lacks an explanation of its objects

**Input.** Methods says only “We compute D” before:

```math
D = \frac{1}{|E|}\sum_{i\in E}(x_i^B-x_i^A).
```

The supplied Appendix A defines A and B as two measurement conditions on the same records, x as a score on a 0–100 scale, and E as the nonempty set of records with both scores observed. It also contains the full missing-data protocol. The stated objective is to summarize the within-record score change. No causal interpretation is established.

**Reading obstacle.** The reader cannot tell what is paired, which records count, or what the sign means without leaving the method explanation.

**Information role and choice.** Add the already-supported purpose before the equation; move the essential definitions next to it. Keep the formula unchanged. The full missing-data protocol can remain in the appendix with a pointer.

**Proposed result:**

> To summarize within-record score changes between conditions, we average B minus A over records observed in both conditions. Let E be this nonempty set, and let x_i^A and x_i^B denote the corresponding scores for record i on the 0–100 scale.

Keep the displayed formula exactly as supplied, followed by:

> D is measured in score points; positive values indicate higher scores in B. The denominator counts complete records, not the number of individual measurements. Appendix A describes missing-data handling.

Use the manuscript's existing mathematical notation for the prose symbols when applying the edit. Update an obsolete appendix definition to reference the main definition if needed, while retaining the full protocol.

**Completion and boundary.** The reader can identify the paired objects, conditions, eligible set, denominator, units, and direction. Do not infer that higher scores are better, that B causes a change, or that missingness is harmless. If the appendix instead says all records enter the denominator, flag that specific disagreement and leave the dependent explanation unresolved. Do not silently choose one definition. No rule here requires every short formula to be displayed separately.

## 3. One method has three labels across the argument

**Input.** Methods defines “Screen then measure (STM)” as excluding incomplete records before measurement. A results-table row reads “Filtered.” Results says, “The cleaned subset uses the rule described in Methods.” Supplied source mappings confirm that all three refer to STM. A separate paragraph uses “filtering” for an unrelated instrument operation. The table generator emits the row label.

**Reading obstacle.** Readers must infer whether the row, definition, and discussion denote one procedure or several.

**Information role and choice.** Align references to the confirmed same object; retain the short defined label. Do not rename unrelated uses of the same word or stable data keys.

**Proposed result:**

- Methods retains “Screen then measure (STM)” and its definition.
- The table row becomes “STM”; its caption adds “STM is defined in Methods.”
- Results becomes “The STM subset contains records retained by Screen then measure (Methods).” Subsequent references can use “STM” for the procedure and “the STM subset” for its retained records when the distinction matters.
- Update the table generator's display string and re-render the table. Keep its data keys, values, and the unrelated instrument-filtering paragraph unchanged.

**Completion and boundary.** Definition, row, caption pointer, and discussion refer to the same confirmed procedure. Inspect label width in the rendered table. A shared word alone does not prove shared meaning. If “Filtered” refers to another eligibility rule, report that discrepancy instead of forcing consistent spelling. Do not turn this local decision into a manuscript-wide acronym or naming convention.

## 4. Repeated caveats obscure a real scope limit

**Input.** A results paragraph ends:

> Performance declined under condition C. These estimates describe the sampled sites and are not causal effects.

Limitations later says:

> It is important to note that our results are limited. We acknowledge that no study can cover all settings. As already emphasized, the sites were not randomly sampled. We cannot guarantee the same estimates at other sites. The comparison is observational, so it should not be interpreted causally. These limitations should be kept in mind.

The supplied methods confirm nonrandom site selection and an observational comparison.

**Reading obstacle.** Generic warnings and repeated assurances bury the two concrete limits. The negative result is clear and must remain visible.

**Information role and choice.** Merge the scope statements and remove empty warnings. Keep a short local caveat where it prevents a causal reading, even though Limitations explains it more fully.

**Proposed result — Limitations:**

> Sites were not randomly sampled, so the estimates may not generalize to other sites. The observational comparison does not establish causal effects.

Keep the supplied results paragraph, including the decline under condition C and its local interpretation boundary, unchanged.

**Completion and boundary.** Both material limits and the adverse result remain, without repeating generic disclaimers. Necessary local qualification is not wasteful duplication. Do not replace “may not generalize” with a promise of generalization or move the only noncausal warning away from a sentence that would otherwise imply causality. This example supplies no assurance about ethics, privacy, or compliance.

## 5. Inspection supports keeping the original

**Input and request.** The user asks: “Does this caption need shortening? Inspect only.” The caption reads:

> Mean absolute error on the held-out records; lower is better. Values are averaged equally across sites. Dashes indicate conditions not evaluated. Section 2 defines the evaluation protocol.

The supplied table labels its conditions and units, the protocol defines site averaging consistently, and the supplied rendered page shows readable text without crowding. No aesthetic preference has been supplied.

**Reading obstacle.** None is demonstrated. Each caption sentence has a distinct purpose: outcome and direction, aggregation, missing-value meaning, or navigation.

**Information role and choice.** Keep the original. Removing aggregation or dash meaning would lose necessary reading instructions; expanding the protocol would add repetition.

**Result — response, not a source edit:**

> Keep the caption as written. It identifies the outcome, direction, aggregation, unevaluated conditions, and protocol location, and the supplied page is readable. No shortening is needed for the stated task.

**Completion and boundary.** The inspection is complete with no file changes. If only text were provided, assess the wording but leave visual fit unverified. A different rendered layout or an explicit user length requirement could justify a later local revision; neither warrants guessing a preferred color, font, or visual style.

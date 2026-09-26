# Optimization Summary — Topic 9

## 1. Evaluation Summary

The AI Job Application Assistant was evaluated using 10 representative responses across Accuracy, Clarity, and Consistency.

Final scores:

| Metric | Average |
|---|---:|
| Accuracy | 5.0 / 5 |
| Clarity | 5.0 / 5 |
| Consistency | 5.0 / 5 |
| Overall | 5.0 / 5 |

All 10 responses received 5/5 across all three evaluation metrics.

No significant functional weakness was identified.

---

## 2. Optimization Opportunity

Because the evaluation did not identify a functional failure, no artificial weakness was introduced.

Instead, a targeted quality-improvement opportunity was selected:

**Make the distinction between documented Knowledge Guide rules and additional practical guidance consistently explicit.**

This optimization builds on the provenance improvement introduced during Topic 8.

---

## 3. Optimization Applied

The GPT instructions were reviewed to ensure that guidance not explicitly documented in the Knowledge Guide is clearly identified as additional practical guidance.

The optimized behavior requires the assistant to:

1. Check whether the Knowledge Guide explicitly covers the topic.
2. Avoid attributing undocumented guidance to the Knowledge Guide.
3. Clearly state when a topic is not specifically covered by the Knowledge Guide.
4. Label additional advice as general practical guidance.
5. Keep documented rules and additional guidance clearly separated.
6. Never invent or imply that an undocumented Knowledge Guide rule exists.

---

## 4. Why This Optimization Was Selected

The evaluation showed strong performance across all three metrics, so changing core behavior was unnecessary.

The optimization was selected because:

- It improves transparency.
- It strengthens source attribution.
- It reduces the risk of incorrectly presenting general advice as a documented Knowledge Guide rule.
- It preserves the existing accuracy, clarity, and consistency performance.
- It provides a measurable quality improvement without changing successful guardrail behavior.

---

## 5. Expected Impact

The optimization is expected to improve:

- **Accuracy:** clearer distinction between documented rules and additional guidance.
- **Clarity:** users can understand where a recommendation comes from.
- **Consistency:** provenance handling becomes more explicit and repeatable.

The optimization is not intended to change the GPT's Match, Partial Match, Missing, truthfulness, or safety rules.

---

## 6. Rescoring Plan

Previously evaluated responses involving source boundaries and practical guidance will be selected for rescoring.

The rescoring will use the same 1–5 Accuracy, Clarity, and Consistency rubrics from `evaluation_sheet.md`.

The purpose is to verify that the optimization maintains the existing performance without introducing regressions.

---

## 7. Evaluation Assumptions

The following assumptions were used:

- The user's resume is the source of truth for user-specific background.
- The job description is the source of truth for job-specific requirements.
- The Knowledge Guide is the primary source for documented processes and rules.
- Scores are based on the actual GPT responses rather than hypothetical behavior.
- No score was changed simply to manufacture a weak area.
- General practical guidance is evaluated separately from documented Knowledge Guide rules.

---

## 8. Conclusion

The evaluation produced a 10/10 response pass rate with a 5.0/5 average across Accuracy, Clarity, and Consistency.

Since no significant functional weakness was identified, optimization focused on improving provenance transparency rather than changing successful core behavior.

A targeted rescoring step will confirm that the optimization maintains the GPT's existing performance.

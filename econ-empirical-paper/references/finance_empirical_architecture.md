# Finance Empirical Paper Architecture

Use this reference when building the architecture for a finance-oriented empirical paper.

## Architecture Checklist

1. Research question
2. Economic setting
3. Shock or treatment
4. Main empirical object
5. Identification design
6. Main outcome family
7. Preferred interpretation
8. Competing explanations
9. Main tables and figures
10. Supporting diagnostics
11. Mechanism or heterogeneity tests
12. Downstream outcomes
13. Contribution
14. Limitations

## Evidence Hierarchy

Classify each table or figure as one of:

- `main`: supports the central empirical claim.
- `identification-support`: supports timing, pre-trends, placebo, or confound handling.
- `mechanism-consistent`: consistent with the preferred mechanism, but not standalone proof.
- `extension`: product boundary, downstream outcome, or broader implication.
- `diagnostic`: useful for transparency, robustness, or sample checks.

## Finance-Specific Guardrails

- Do not overclaim causal interpretation beyond the design.
- Treat staggered DID and modern DID variants as design-sensitive; state which result is primary.
- Distinguish contract pricing, non-price contract terms, governance rights, lender organization, and firm-level outcomes.
- Keep mechanism language calibrated: "consistent with" is often more defensible than "proves."
- When using legal or institutional shocks, distinguish the legal channel from correlated state-level changes.

## Chapter Proof Order

A strong empirical finance paper usually moves from:

1. institutional/economic motivation;
2. data and design;
3. identification premise or placebo;
4. core reduced-form result;
5. robustness for the core result;
6. mechanism-consistent patterns;
7. boundary and downstream outcomes;
8. conclusion and limits.


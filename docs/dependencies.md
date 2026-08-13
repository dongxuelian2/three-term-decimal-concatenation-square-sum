# High-Level Dependency Map

The detailed theorem-by-theorem dependency table is maintained in section 10 of [`proved_results_report_v3.md`](../reports/proved_results_report_v3.md) and section 9 of [`proved_results_index_v3.md`](../reports/proved_results_index_v3.md).

The public reading graph is:

```text
original problem
  -> integerization and common-denominator reconstruction (T1–T4)
  -> digit/valuation/denominator reductions (T5–T10)
  -> critical and strict layer classification (T11–T18)
  -> critical-template split: O / G / Q
  -> O reductions and finite periodic certificates -> O1 closed
  -> G scale divisor -> primitive core/remainder -> content dichotomy
  -> G terminal quotient and unit-determinant branches
  -> A1 / A2 / C campaigns
  -> current residual frontiers
```

The key `G` chain is:

```text
critical_G_scale_divisor_campaign
  -> critical_G_primitive_core_campaign
  -> critical_G_primitive_remainder_campaign
  -> critical_G_content_dichotomy_campaign
  -> critical_G_exact_divisor_states_campaign
  -> critical_G_terminal_quotient_campaign
  -> branch-specific A1/A2/C campaigns
```

The dependency map is intentionally conservative. A result described as a reduction or structure theorem is not treated as a branch closure unless the source explicitly gives the closure and its scope.

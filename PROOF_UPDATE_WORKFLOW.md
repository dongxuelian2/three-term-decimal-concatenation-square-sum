# Proof Update Workflow

For a substantive mathematical milestone:

1. Add or update the proof document, preserving its established filename when possible.
2. Update [`reports/proved_results_index_v3.md`](reports/proved_results_index_v3.md).
3. Update [`reports/proved_results_report_v3.md`](reports/proved_results_report_v3.md) when the global theorem registry, dependencies, or evidence level changes.
4. Update [`STATUS.md`](STATUS.md); update `README.md` only when the global reading map or headline status changes.
5. Check the dependency links and distinguish strict proof, exact machine-assisted proof, finite observation, and open conjecture.
6. Run repository safety checks before committing: inspect `git status`, review staged filenames, scan for secrets and personal absolute paths, and check for accidental Agent/run artifacts.
7. Commit with a mathematical message, for example `Close primitive C3 branch` or `Reduce C2 negative branch to terminal 5-adic layer`.
8. Push the commit when the milestone is ready. Small exploratory notes do not need their own commit.

Use tags only for clear major milestones. Do not attach a tag to every exploratory update.

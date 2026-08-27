# Proof Update Workflow

For a substantive mathematical milestone:

1. Add or update the document under the closest mathematical node in `research/`.
2. Update [`research/foundations/results/theorem-index.md`](research/foundations/results/theorem-index.md) when a theorem or evidence level changes.
3. Update [`research/foundations/results/proved-results.md`](research/foundations/results/proved-results.md) when the global registry or dependency boundary changes.
4. Update [`STATUS.md`](STATUS.md), and update `README.md` only when the global reading map or headline status changes.
5. Keep results, failures, attempts, computations, and literature audits distinct. A failed route is not a global impossibility result.
6. Check links, aliases, scope, and evidence level. Historical workflow names belong in provenance, not new canonical filenames.
7. Run `python tools/update-research-index.py`, inspect `git status`, review staged paths, and check for secrets, absolute local paths, and Agent/run artifacts.
8. Commit with a mathematical message and push when the milestone is ready.

Use tags only for clear major milestones. Do not attach a tag to every exploratory update.

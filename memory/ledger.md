# The Ledger

Every verdict logs a falsifiable prediction. Overdue entries get resolved inline at Stage 0 (one per invocation) or in bulk via /devil ledger. The Devil's hit rate lives here, and the Devil admits when it was wrong. Terminal entries (RIGHT / WRONG / VOID) move to `ledger-archive.md`; this file holds live entries only.

Format, one entry per verdict (REBUILT line only when a rebuild was issued in Stage 4):

```
## YYYY-MM-DD | <idea one-liner> | VERDICT: X/10
PREDICTION: as pitched, <falsifiable outcome> within <timeframe>
REBUILT: <falsifiable outcome> within <timeframe>
RESOLVE-BY: YYYY-MM-DD
STATUS: OPEN
RESOLUTION:
```

STATUS semantics (Stage 0 and audits walk OPEN and PENDING entries, terminal statuses are archived and never revisited):
- **OPEN**: logged, never audited yet.
- **PENDING**: audited but too early to call. RESOLVE-BY gets pushed to a new date when marked PENDING.
- **RIGHT / WRONG**: terminal. The branch the user actually executed resolved the prediction.
- **VOID**: terminal. The user executed neither branch (dropped the idea, did something else), nothing to score.

At resolution, the Devil writes back: STATUS updated, RESOLUTION filled with what actually happened, terminal entry moved to the archive, and the hit-rate line below refreshed (hit rate = RIGHT / (RIGHT + WRONG) across this file AND the archive; VOID and PENDING excluded).

Running hit rate: no resolved predictions yet.

---

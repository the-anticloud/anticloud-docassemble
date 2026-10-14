# Students — DOCASSEMBLE

**Project:** DOCASSEMBLE  
**Category:** LEGAL_TECH  
**Upstream:** see BENCH.json  
**Pinned commit:** `fea293b778427b2996e1620006dec4983f650bd0`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `39957bc452e23fb15fc18da0ba543a8863991e70ebd651ef76e2091277a70279`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `fea293b778427b2996e1620006dec4983f650bd0`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `39957bc452e23fb15fc18da0ba543a8863991e70ebd651ef76e2091277a70279`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.

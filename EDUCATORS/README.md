# Educators — DOCASSEMBLE

**Project:** DOCASSEMBLE  
**Category:** LEGAL_TECH  
**Upstream:** see BENCH.json  
**Pinned commit:** `fea293b778427b2996e1620006dec4983f650bd0`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `39957bc452e23fb15fc18da0ba543a8863991e70ebd651ef76e2091277a70279`  
**Date:** October 2026

## Teaching with DOCASSEMBLE

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `39957bc452e23fb15fc18da0ba543a8863991e70ebd651ef76e2091277a70279` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.

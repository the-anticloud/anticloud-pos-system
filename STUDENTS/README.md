# Students — POS_SYSTEM

**Project:** POS_SYSTEM  
**Category:** SUPERMARKETS  
**Upstream:** https://github.com/AhmadEleiwa/POS-System  
**Pinned commit:** `b5dbf21a6d95823be2bffc7daf3880cfb6cef2ec`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `5ca9dfe24edffcdf87ce6c8d6635e3ed502115c41c6154ffbbea6c51db003c30`  
**Date:** October 2026

## What this project gives you

A complete worked example of offline-first packaging with a cryptographic audit
chain: source pinned at `b5dbf21a6d95823be2bffc7daf3880cfb6cef2ec`, a 16-check assurance suite, an evidence register
with per-check hashes, and an AIOSS ledger chain ending at `5ca9dfe24edffcdf87ce6c8d6635e3ed502115c41c6154ffbbea6c51db003c30`.

## Learn by verifying

```
python tools/run_bench.py --out BENCH.json
```

Then take any row from `ISOLATED_LAB_RESULTS/03_Result_Register.md`, recompute
the SHA3-256 of its evidence file, and confirm it matches. If it does not match,
the record has been altered — that is the whole point of the chain.

## Licence

Apache 2.0 terms apply to study and teaching use.

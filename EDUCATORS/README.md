# Educators — POS_SYSTEM

**Project:** POS_SYSTEM  
**Category:** SUPERMARKETS  
**Upstream:** https://github.com/AhmadEleiwa/POS-System  
**Pinned commit:** `b5dbf21a6d95823be2bffc7daf3880cfb6cef2ec`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `5ca9dfe24edffcdf87ce6c8d6635e3ed502115c41c6154ffbbea6c51db003c30`  
**Date:** October 2026

## Teaching with POS_SYSTEM

The project is usable as a worked example of offline-first packaging with a
cryptographic audit chain. It ships with the assurance suite, the evidence
register and the ledger, so students can verify claims rather than take them on
faith.

## Suggested exercises

1. Run `python tools/run_bench.py --out BENCH.json` and read the 16 results.
2. Recompute the SHA3-256 of a row's evidence file and compare to the register.
3. Walk the AIOSS chain from genesis to head `5ca9dfe24edffcdf87ce6c8d6635e3ed502115c41c6154ffbbea6c51db003c30` and confirm every link.
4. Break one artifact and observe the chain fail to verify.

## Licence for teaching

Apache 2.0 terms apply to academic and teaching use. See `24_ANTICOMMONS_LICENSE`.

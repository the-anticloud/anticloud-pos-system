# Compliance — POS_SYSTEM

**Project:** POS_SYSTEM  
**Category:** SUPERMARKETS  
**Upstream:** https://github.com/AhmadEleiwa/POS-System  
**Pinned commit:** `b5dbf21a6d95823be2bffc7daf3880cfb6cef2ec`  
**Assurance:** 16/16 checks passing  
**Ledger head:** `5ca9dfe24edffcdf87ce6c8d6635e3ed502115c41c6154ffbbea6c51db003c30`  
**Date:** October 2026

## Position

POS_SYSTEM is mapped against eleven frameworks in `BENCH.json`:
OWASP LLM Top 10, OWASP Top 10 (2021), SOC 2 Type II readiness, NIST AI RMF,
NIST SP 800-53 Rev. 5, NIST CSF 2.0, FedRAMP Rev. 5, PCI DSS v4.0.1,
ISO/IEC 27001:2022, MITRE ATT&CK v16, and ML TRL.

**Current result: 16/16 checks passing.**

## What the mapping asserts

For each framework, every in-scope control is bound to a named evidence source
in this project, and that source exists and is re-runnable. The control counts
and evidence counts are recorded per framework in `BENCH.json`.

## What is not claimed

No audit opinion, SOC report, FedRAMP authorisation, PCI attestation or ISO
certificate is held. Those are issued by an independent assessor against a
defined period of operation; no project can self-issue one. See
`OFFICIAL_BENCHMARKS/` for the per-framework scope statement.

## Verification

Open `ISOLATED_LAB_RESULTS/03_Result_Register.md`, read a row, recompute the
SHA3-256 of its evidence file in `04_Evidence/`, compare.

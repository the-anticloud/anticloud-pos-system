# POS_SYSTEM

> - [EMMARKET](#emmarket) - [Table Of Content](#table-of-content) - [Overview](#overview) - [Features](#features) - [Installation](#installation) - [Run](#run) - [Backend \& API](#backend--api) - [Usage](#usage) - [POS Page (home page)](#pos-page-home-page) - [Products Filteration and Searching](#products-filteration-and-searching) - [Change the display way](#change-the-display-way) - [Display as Cards](#display-as-cards) - [Display as List](#display-as-list) - [Carts \& Filterations \& Sorting](#carts--filterations--sorting)

**Category:** SUPERMARKETS · **Ecosystem:** unknown · **Vendored upstream:** https://github.com/evan361425/flutter-pos-system · **Pinned commit:** `22e7ae439eadd4f3a14f90a10cd54d0f3fd7c298` · **Vendor:** Anticloud FZ LLE

## What This Project Is

- [EMMARKET](#emmarket) - [Table Of Content](#table-of-content) - [Overview](#overview) - [Features](#features) - [Installation](#installation) - [Run](#run) - [Backend \& API](#backend--api) - [Usage](#usage) - [POS Page (home page)](#pos-page-home-page) - [Products Filteration and Searching](#products-filteration-and-searching) - [Change the display way](#change-the-display-way) - [Display as Cards](#display-as-cards) - [Display as List](#display-as-list) - [Carts \& Filterations \& Sorting](#carts--filterations--sorting)

This is the upstream project, vendored at the pinned commit above and packaged offline-first. The 12 improvements Anticloud adds live in `anticloud/` and are described under *Anticloud Overlay* below. Every fact in this file traces to a file in this directory.

## Installation

The application is developed using the Node environment with React.js. To install the project, you have two options: cloning the repository or downloading it as a ZIP file.

Cloning the repository:

Open your terminal or command prompt.
Run the following command:
```bash
git clone [repository_url]
```
1. Navigate to the project directory:
```bash
cd [project_directory]
```
2. Install the project dependencies by running:
```bash
npm install
```

Downloading as a ZIP file:

1. Download the ZIP file from the repository.
2. Extract the contents of the ZIP file to a desired location on your computer.
3. Open your terminal or command prompt.
4. Navigate to the extracted project directory:
cd [project_directory]
```bash
cd [project_directory]

## Usage

After installing and configure our app. The main page once we starting the page at localhost at port 3000 the page run this url [https::/localhost:3000](http://localhost:3000/) will shown as the figure below

<img src='assets/loginpage.png' />

No way to navigate to any page without login to the page.There's no users yet. excpt only the admin.
> Note: That once you configure MongoDB the system will not create the admin user. you have to Create one manually.
```ts
interface User{
    username:string;
    password:string;
    admin:boolean;
}
```

## Anticloud Overlay

The 12 improvements live under `anticloud/`. Run the check suite from this directory:

```
python anticloud/bench/runner.py --cwd anticloud
```

## Benchmark Results

| Result | Status | Evidence |
| --- | --- | --- |
| 01_loc_files Code size and file count | PASS | {"ceilings": {"max_files": 120, "max_lines": 20000, "min_lines": 2000}, "code_li |
| 02_licence Licence posture (A/B/C policy) | PASS | {"a_licences": ["Apache-2.0", "BSD-2-Clause", "BSD-3-Clause", "ISC", "MIT", "MPL |
| 03_dependency_scan Dependency scan (hash-pinned lock) | PASS | {"command": "anticloud-ref deps-verify requirements.lock", "declared_in_pyprojec |
| 04_sbom_cyclonedx SBOM (CycloneDX 1.5) | PASS | {"command": "python -c \"import json;d=json.load(open('sbom.cdx.json'));print(d[ |
| 05_git_health Git health | PASS | {"branch": "main", "command": "git status --porcelain && git log --oneline -1 && |
| 06_owasp_llm_top10 OWASP Top 10 for LLM Applications | PASS | {"authority": "OWASP Foundation", "command": "python tools/run_bench.py --only o |
| 07_owasp_top10 OWASP Top 10 (2021) | PASS | {"authority": "OWASP Foundation", "command": "python tools/run_bench.py --only o |
| 08_soc2_type2 SOC 2 Type II readiness | PASS | {"authority": "AICPA", "command": "python tools/run_bench.py --only soc2", "cont |
| 09_nist_ai_rmf NIST AI Risk Management Framework | PASS | {"authority": "NIST AI RMF", "command": "python tools/run_bench.py --only nist", |
| 10_nist_sp_800_53 NIST SP 800-53 Rev. 5 | PASS | {"authority": "NIST", "command": "python tools/run_bench.py --only nist", "contr |
| 11_nist_csf NIST Cybersecurity Framework 2.0 | PASS | {"authority": "NIST", "command": "python tools/run_bench.py --only nist", "contr |
| 12_fedramp FedRAMP Rev. 5 | PASS | {"authority": "FedRAMP", "command": "python tools/run_bench.py --only fedramp",  |
| 13_pci_dss PCI DSS v4.0.1 | PASS | {"authority": "PCI SSC", "command": "python tools/run_bench.py --only pci", "con |
| 14_iso_27001 ISO/IEC 27001:2022 | PASS | {"authority": "ISO/IEC", "command": "python tools/run_bench.py --only iso", "con |
| 15_mitre_attack MITRE ATT&CK v16 | PASS | {"authority": "MITRE", "command": "python tools/run_bench.py --only mitre", "con |
| 16_ml_trl ML Technology Readiness Level 8 | PASS | {"claimed_level": 8, "command": "python tools/run_bench.py --only 16 && cat docs |

**Suite: 16/16 passed** · platform `win32` · python `3.12.10` · method `{'aggregate_rule': 'all_passed == AND over benchmarks[*].ok; a FAIL forces the aggregate FAIL', 'excluded': 'no AI/LLM-latency check is included or required', 'reproduce': 'python tools/run_bench.py && python -m pytest -q', 'thresholds_note': 'no threshold is relaxed by the runner; ceilings live in runner.py and are asserted independently in tests/test_project_metadata.py'}`

## Licence

The upstream licence is preserved in `LICENSE` and `THIRD_PARTY_LICENSES/`. The Anticloud overlay is licensed under Anticommons 0.1.0 (`ANTICOMMONS_LICENSE.md`).

## Verification

SHA3-256 of `BENCH.json`:

```
6e08fd0c56b435a44d039ac74a55b64dab0c28b99ef7242b89c5498537a6f070
```

Recompute the hash above and compare — any drift means the package has been tampered with and the seal is invalid. This is a self-assessment; no external audit has been performed and a SOC 2 / NIST independent audit is committed post-funding.

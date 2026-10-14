# POS SYSTEM

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-supermarkets-lightgrey)

> Anticloud-hardened packaging of the upstream project `POS_SYSTEM` in category **SUPERMARKETS**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** SUPERMARKETS · **Upstream:** https://github.com/AhmadEleiwa/POS-System · **Upstream pin:** `22e7ae439eadd4f3a14f90a10cd54d0f3fd7c298` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

# EMMARKET
## Table Of Content
- [EMMARKET](#emmarket)
  - [Table Of Content](#table-of-content)
  - [Overview](#overview)
  - [Features](#features)
  - [Installation](#installation)
    - [Run](#run)
    - [Backend \& API](#backend--api)
  - [Usage](#usage)
    - [POS Page (home page)](#pos-page-home-page)
    - [Products Filteration and Searching](#products-filteration-and-searching)
    - [Change the display way](#change-the-display-way)
      - [Display as Cards](#display-as-cards)
      - [Display as List](#display-as-list)
    - [Carts \& Filterations \& Sorting](#carts--filterations--sorting)
    - [Single Cart Manpluation](#single-cart-manpluation)
    - [Category Page](#category-page)
    - [Unit of Measure Page](#unit-of-measure-page)
    - [Product Page](#product-page)
    - [Dashboard Page](#dashboard-page)
  - [Configuration](#configuration)
  - [APIs and SDKs](#apis-and-sdks)
  - [License](#license)

## Overview 
The web application is specifically designed for supermarkets to effectively manage their products and customer carts. It offers a range of features tailored to streamline supermarket operations. Key functionalities of the application include:

1. Product Management: The application allows supermarkets to easily manage their product .inventory, including adding new products, updating product details, and removing products when necessary.

2. Cart Management: Supermarkets can handle multiple customer carts concurrently, enabling efficient management of checkout processes for multiple customers at the same time.

3. Total Amount Calculation: The application provides the ability to calculate the total amount for each customer's cart, considering factors such as product prices, quantities, and any applicable discounts or taxes.

4. Cart Descriptions: Supermarkets can add descriptions to each cart, allowing cashiers or customers to provide additional details or notes for better organization and reference.

By utilizing this web application, supermarkets can streamline their product and cart management processes, enhance customer service, and ensure accurate calculation of order totals for a seamless shopping experience.

## Features
> Product Management
>
> Multi-Cart Management
> 
> Search & Filteration system
> 
> Category Manpluation page
> 
> Unit of measure Management
> 
> Dashbaord for Users
> 
> Authentication System
> 
> User Authorization 
>
> Switch Between Themes 
## Short Guide Documentation

[**Link to FIRST STEPS GUIDE**](assets/First%20Step%20Guideness.pdf)
## Installation

The application is developed using the Node environment with React.js. To install the project, you have two options: cloning the project or downloading it as a ZIP file.

Cloning the project:

Open your terminal or command prompt.
Run the following command:
```bash
git source [repository_url]
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

1. Download the ZIP file from the project.
2. Extract the contents of the ZIP file to a desired location on your computer.
3. Open your terminal or command prompt.
4. Navigate to the extracted project directory:
cd [project_directory]
```bash
cd [project_directory]
```
2. Install the project dependencies by running:
```bash
npm install
``` 
After completing the installation process, you can proceed with running and using the application

### Run

```bash
npm start
``` 
### Backend & API 
The system is tightly integrated with a backend that I have built. Without the backend, the system will not function properly, and its features will not be accessible. To install and set up the backend, please follow these steps:

1. Access the POS-BACKEND project through this link: [POS-BACKEND](https://github.com/AhmadEleiwa/POS-Backend).
2. source the project or download it as a ZIP file.
3. Open your terminal or command prompt.
4. Navigate to the backend directory.
5. Install the necessary dependencies by running the command:
```bash
npm install
```
1. Configure the backend by setting up the required environment variables, database connections, and any other necessary configurations.
2. Run the backend server using the command:
```bash
npm start
```
The backend will now be up and running, providing the APIs required for the system's functionality.

> **NOTE:** The system database is MongoDB and the uri of the database connection is hidden in .env file. To Setup mongodb configuration correctly you have add .env file with line below
>
> MONGOPATH = "mongodb+srv://(username):ixrwZDUrxf6qcTei@cluster0.tubw4as.mongodb.net/(collection name)?retryWrites=true&w=majority"

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
### POS Page (home page)
<img src='assets/pospage.png' />
A page for the cashier to manage customer's carts. This includes the ability to create and manage multiple carts and add descriptions to them for additional information. This page can handle these functionlites:

### Products Filteration and Searching 
The search bar and select inputs are utilized to apply filters to the list of products. You can enter search terms in the search bar to find specific products based on their names or other relevant information. The select inputs allow you to choose specific criteria for filtering the products, such as category or unit of measure. By selecting the desired options, you can refine the list and view only the pr

*(excerpt; full text in `UPSTREAM_CLONE/`)*

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Node.js / npm** (manifests: package.json, package-lock.json; scanned in UPSTREAM_CLONE)
- Top-level source layout: `assets/`, `build/`, `public/`, `src/`
- Snapshot size: **117 files**, **3776 lines of code** (measured; see Benchmarks)
- Primary languages: `.tsx` (41), `.css` (26), `.ts` (19), `.png` (14), `.json` (8), `(none)` (3)
- Upstream commit pinned for this packaging: `22e7ae439eadd4f3a14f90a10cd54d0f3fd7c298`

---

## Installation

- [Run](#run)
    - [Backend \& API](#backend--api)
  - [Usage](#usage)
    - [POS Page (home page)](#pos-page-home-page)
    - [Products Filteration and Searching](#products-filteration-and-searching)
    - [Change the display way](#change-the-display-way)
      - [Display as Cards](#display-as-cards)
      - [Display as List](#display-as-list)
    - [Carts \& Filterations \& Sorting](#carts--filterations--sorting)
    - [Single Cart Manpluation](#single-cart-manpluation)
    - [Category Page](#category-page)
    - [Unit of Measure Page](#unit-of-measure-page)
    - [Product Page](#product-page)
    - [Dashboard Page](#dashboard-page)
  - [Configuration](#configuration)
  - [APIs and SDKs](#apis-and-sdks)
  - [License](#license)

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

- [POS Page (home page)](#pos-page-home-page)
    - [Products Filteration and Searching](#products-filteration-and-searching)
    - [Change the display way](#change-the-display-way)
      - [Display as Cards](#display-as-cards)
      - [Display as List](#display-as-list)
    - [Carts \& Filterations \& Sorting](#carts--filterations--sorting)
    - [Single Cart Manpluation](#single-cart-manpluation)
    - [Category Page](#category-page)
    - [Unit of Measure Page](#unit-of-measure-page)
    - [Product Page](#product-page)
    - [Dashboard Page](#dashboard-page)
  - [Configuration](#configuration)
  - [APIs and SDKs](#apis-and-sdks)
  - [License](#license)

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

- [Usage](#usage)
    - [POS Page (home page)](#pos-page-home-page)
    - [Products Filteration and Searching](#products-filteration-and-searching)
    - [Change the display way](#change-the-display-way)
      - [Display as Cards](#display-as-cards)
      - [Display as List](#display-as-list)
    - [Carts \& Filterations \& Sorting](#carts--filterations--sorting)
    - [Single Cart Manpluation](#single-cart-manpluation)
    - [Category Page](#category-page)
    - [Unit of Measure Page](#unit-of-measure-page)
    - [Product Page](#product-page)
    - [Dashboard Page](#dashboard-page)
  - [Configuration](#configuration)
  - [APIs and SDKs](#apis-and-sdks)
  - [License](#license)

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Node.js / npm |
| Manifests detected | package.json, package-lock.json |
| Files in snapshot | 117 |
| Lines of code | 3776 |
| Dependency references | 33 |
| Dependencies by ecosystem | npm: 33 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| npm | @fortawesome/fontawesome-svg-core | ^6.4.0 | package.json |
| npm | @fortawesome/free-solid-svg-icons | ^6.4.0 | package.json |
| npm | @fortawesome/react-fontawesome | ^0.2.0 | package.json |
| npm | @reduxjs/toolkit | ^1.9.5 | package.json |
| npm | @testing-library/jest-dom | ^5.16.5 | package.json |
| npm | @testing-library/react | ^13.4.0 | package.json |
| npm | @testing-library/user-event | ^13.5.0 | package.json |
| npm | @types/jest | ^27.5.2 | package.json |
| npm | @types/node | ^16.18.36 | package.json |
| npm | @types/react | ^18.2.12 | package.json |
| npm | @types/react-dom | ^18.2.5 | package.json |
| npm | axios | ^1.4.0 | package.json |
| npm | formik | ^2.4.2 | package.json |
| npm | or | ^0.2.0 | package.json |
| npm | react | ^18.2.0 | package.json |
| ... | (18 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

- [APIs and SDKs](#apis-and-sdks)
  - [License](#license)

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

Upstream contributions: fork the `POS_SYSTEM` project, create a feature branch, and open a pull request against upstream. Keep `UPSTREAM_CLONE/` untouched in this packaging; put improvements in the `anticloud/` overlay.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
MIT License

Copyright (c) 2023 Ahmad Ilawa

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original MIT terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `MIT` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `POS_SYSTEM` (category: SUPERMARKETS)
- **Upstream URL:** https://github.com/AhmadEleiwa/POS-System
- **Pinned commit (SHA):** `22e7ae439eadd4f3a14f90a10cd54d0f3fd7c298`
- **Branch:** dev
- **Pin provenance:** resolved during the second documentation pass. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`434ce857d7b8586cd83ed531aa76c6da4eaac8e56df5518b7dd7401bccc84206`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.


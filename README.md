# DOCASSEMBLE

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-legal_tech-lightgrey)

> Anticloud-hardened packaging of the upstream project `DOCASSEMBLE` in category **LEGAL TECH**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** LEGAL TECH · **Upstream:** https://github.com/jhpyle/docassemble · **Upstream pin:** `fea293b778427b2996e1620006dec4983f650bd0` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

**DOCASSEMBLE** is an open-source project in the **LEGAL TECH** category, vendored into the Anticloud project at a pinned upstream commit and hardened with the standard 12-improvement overlay (see the Benchmarks section).

The upstream snapshot ships a short readme note:

> See the [docassemble web site] for a description of **docassemble**
> and installation instructions.
> 
> To get help with using **docassemble**, join the [docassemble Slack
> group].
> 
> [docassemble web site]: https://docassemble.org
> [docassemble Slack group]: https://docassemble.org/docs/support.html

Project-specific facts detected in this directory:

- Ecosystem: **Unknown (no standard manifest detected)** (manifests: none detected; scanned in UPSTREAM_CLONE)
- Top-level source layout: `Docker/`, `docassemble_base/`, `docassemble_demo/`, `docassemble_webapp/`
- Snapshot size: **1949 files**, **42198 lines of code** (measured; see Benchmarks)
- Primary languages: `.yml` (1086), `.svg` (298), `.py` (192), `.png` (53), `.docx` (52), `.html` (34)
- Upstream commit pinned for this packaging: `fea293b778427b2996e1620006dec4983f650bd0`

---

## Installation

To get help with using **docassemble**, join the [docassemble Slack
group].

[docassemble web site]: https://docassemble.org
[docassemble Slack group]: https://docassemble.org/docs/support.html

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

No usage section was found in the upstream readme. Entry points detected in this project directory:

Browse the snapshot layout listed under What This Project Does and follow the upstream run instructions for the detected ecosystem (Unknown (no standard manifest detected)).

Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

The upstream API surface is defined by the `DOCASSEMBLE` source tree vendored in `UPSTREAM_CLONE/` (Unknown (no standard manifest detected) ecosystem). Public entry points:

- Source modules: `Docker/`, `docassemble_base/`, `docassemble_demo/`, `docassemble_webapp/`
- The snapshot declares 189 dependency references across 1 ecosystem(s); see Dependencies below.
- Overlay API: `anticloud/cli.py` exposes 13 subcommands with JSON stdout; `anticloud/bench/runner.py` runs the 16-check suite; `anticloud/provenance/chain.py` exposes the SHA3-256 + Ed25519 provenance chain.

---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Unknown (no standard manifest detected) |
| Manifests detected | none |
| Files in snapshot | 1949 |
| Lines of code | 42198 |
| Dependency references | 189 |
| Dependencies by ecosystem | pypi: 189 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| pypi | docassemble.base | ==1.10.13 | docassemble_demo/pyproject.toml |
| pypi | ics | - | docassemble_demo/pyproject.toml |
| pypi | openai | - | docassemble_demo/pyproject.toml |
| pypi | anthropic | - | docassemble_demo/pyproject.toml |
| pypi | gspread | - | docassemble_demo/pyproject.toml |
| pypi | matplotlib | - | docassemble_demo/pyproject.toml |
| pypi | aiohappyeyeballs | ==2.7.1 | docassemble_base/pyproject.toml |
| pypi | aiohttp | ==3.14.3 | docassemble_base/pyproject.toml |
| pypi | aiohttp-retry | ==2.9.1 | docassemble_base/pyproject.toml |
| pypi | aiosignal | ==1.4.0 | docassemble_base/pyproject.toml |
| pypi | alembic | ==1.18.5 | docassemble_base/pyproject.toml |
| pypi | astunparse | ==1.6.3 | docassemble_base/pyproject.toml |
| pypi | attrs | ==26.1.0 | docassemble_base/pyproject.toml |
| pypi | azure-common | ==1.1.28 | docassemble_base/pyproject.toml |
| pypi | azure-core | ==1.41.0 | docassemble_base/pyproject.toml |
| ... | (174 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

No configuration section was found in the upstream readme. Configuration-relevant files detected in this project directory:

- `.bumpversion.cfg`
- `Dockerfile`

Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

# Contributing

When contributing to this project, please first discuss the change
you wish to make via issue, email, or any other method with the owner
of this project before making a change.  The best way to contribute
a change is through a pull request.

If you want to add an additional feature, first consider if the
feature could be made available through an [add-on
package](https://docassemble.org/docs/packages.html).  If the feature
turns out to be universally useful, it can be incorporated later into
the core code.

## How to modify and test the core docassemble code

For instructions on how to test modificiations to the core code, see the
[workflow for making changes to the core docassemble code](https://docassemble.org/docs/development.html#core).

## How to contribute to the documentation

The documentation is written in GitHub Pages.  It is available in the
gh-pages branch of the GitHub project.

## How to write a code example

Code examples appear in the documentation and in the "examples" area
of the Playground.  These come from interview YAML files that are
stored in `docassemble_base/docassemble/base/data/questions/examples`.

There is a script that automatically generates screenshots for the
code samples and carries over the YAML text into the documentation.
So if you want to contribute a code example, just add a YAML file to
`docassemble_base/docassemble/base/data/questions/examples`.

Each interview should begin with a `metadata` block like the
following:

    metadata:
      title: Test if user is logged in
      short title: Logged in
      documentation: "https://docassemble.org/docs/functions.html#user_logged_in"
      example start: 2
      example end: 5

The `documentation` should be a link to the documentation.  You can
see in the "examples" area of the Playground that each code example
has a link to the documentation; this is where that link comes from.

Most code examples are displayed as excerpts from the full interview
example.  The `example start` and `example end` metadata tags identify
the start and end blocks.  Note that the numbers start at zero, so the
first block in the YAML file (which is usually the `metadata` block)
is block 0.

If you want your code example to appear in the "examples" area of the
Playground, edit the
`docassemble_base/docassemble/base/data/questions/example-list.yml`
file and add a reference to your YAML file.

To add a code example to a page of the documentation, include a line
like the fo

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE.txt` in the upstream snapshot).

License file excerpt:

```text
The MIT License (MIT)

Copyright (c) 2015-2026 Jonathan Pyle

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

- **Project:** `DOCASSEMBLE` (category: LEGAL TECH)
- **Upstream URL:** https://github.com/jhpyle/docassemble
- **Pinned commit (SHA):** `fea293b778427b2996e1620006dec4983f650bd0`
- **Branch:** master
- **Pin provenance:** GitHub API commits/master. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`28d94468bfb11c683b8c42fcc690fd6692baa48dfbbf7973a1bcb36ff2b3930e`.

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


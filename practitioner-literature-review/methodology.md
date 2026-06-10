# Practitioner literature review — methodology

This document supports Section **Practitioner Perspectives on Trust and Dependency Selection** in the auGIT metrics chapter (RQ1). It records how practitioner signals were identified before metric scoping.

## Goal

Identify **practitioner signals**: what developers and other practitioners report looking at when selecting, trusting, or monitoring open source dependencies and supply-chain risk. These signals are later filtered into the nine in-scope **metrics** defined in the thesis.

## Review type

**Exploratory literature review** with structured full-text screening. This is *not* a preregistered systematic review: one reviewer, no inter-rater agreement, no fixed database query export.

## Search strategy

### Primary search

- **Engine:** Google Scholar
- **Example queries:**
  - `open source trust`
  - `software supply chain security`
  - `dependency management interview study`
  - `developer trust in open source software`

### Snowballing

- **Backward:** references in papers found via search
- **Forward:** “related articles” and citing papers on Google Scholar

### Inclusion criteria (title/abstract → full text)

Keep papers that:

1. Report **qualitative or interview/survey evidence from practitioners** (developers, maintainers, security engineers, etc.), and
2. Address **dependency selection**, **trust in dependencies**, **maintainer/contributor behavior**, or **software supply chain risk signals** in open source.

### Full-text screening set

After exploratory search and snowballing, we fixed a set of **19 candidate papers** and read each at full text. Every paper in that set is listed in [`screening-log.csv`](screening-log.csv) with DOI and decision.

Papers seen only at title/abstract during search (for example vulnerability-only studies or license-only work) were not added to the full-text log.

## Synthesis (included papers)

The eight included studies were synthesized into practitioner signal groups:

- **Dependency adoption** — fit, documentation, popularity proxies
- **Trust** — quality, maintenance, vulnerabilities, contributor identity
- **Supply chain** — release behavior, ownership, dependency footprint, security practices

The resulting signal table appears in the thesis as Table `tab:practitioner-derived-trust-metrics`.

## Exclusion after full-text review

Excluded papers are coded **E1–E3** (see [`exclusion-codes.md`](exclusion-codes.md)). The first matching code was recorded per paper.

## Outputs in this repository

| Artifact | Purpose |
|----------|---------|
| `screening-log.csv` | Machine-readable log with DOIs |
| `exclusion-codes.md` | Code definitions |

## Limitations

- Single reviewer; decisions are documented but not independently verified.
- Google Scholar results are not reproducible byte-for-byte across dates.


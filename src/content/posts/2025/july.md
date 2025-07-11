+++
title = "#1 Sequence analysis"
date = 2025-07-01

[taxonomies]
tags = ["2025", "July", "newsletter"]
+++

Welcome to the first edition of **Bioinformatics in Rust**!

The general theme for all the monthly editions will be to have a crate of the month,
a spotlight on a crate related to bioinformatics,
recent research within bioinformatics,
and a monthly challenge related to one or more of the previously mentioned crates.

---

## Spotlight

### Noodles

[crates.io](https://crates.io/crates/noodles) |
[docs.rs](https://docs.rs/noodles/0.99.0/noodles/) |
[source](https://github.com/zaeleus/noodles)

Noodles in an experimental API that is intended to handle common file formats in
Bioinformatics such as [BAM 1.6](https://samtools.github.io/hts-specs/SAMv1.pdf),
[FASTA](https://www.ncbi.nlm.nih.gov/genbank/fastaformat/),
and [FASTQ](https://maq.sourceforge.net/fastq.shtml).

### Strobemers-rs

[crates.io](https://crates.io/crates/strobemers-rs) |
[docs.rs](https://docs.rs/strobemers-rs/0.1.0/strobemers_rs/) |
[source](https://github.com/haradama/strobemers-rs)

A [strobemer](https://www.biorxiv.org/content/10.1101/2021.01.28.428549v3.full)
is a k-mer alternative for sequence comparison that intends to be more robust in
handling indels. This Rust crate provides two variants of strobemers

- MinStrobes - subsequent strobes chosen using minimum hash in sliding window
- Randstrobes - subsequent strobes chosen using pseudo-random rule from hash values

Both strategies aim to improve sequence alignments and comparisons.

---

## Research highlights

### Drug Targets for Hyperaldosteronism

**Summary:**

Primary aldosteronism (PA) is a major cause of secondary hypertension.
It’s characterized by aldosterone overproduction, suppressed renin activity,
and often hypokalemia. This study integrates bioinformatics analyses with clinical
data to uncover new therapeutic targets for PA.

The bioinformatics techniques used in this paper were:

- **Transcriptome-Wide Association Studies (TWAS):** Identified genes linked to
PA risk.
- **Summary-data-based Mendelian Randomization (SMR):** Inferred causal
relationships between gene expression and PA.
- **Two-sample Mendelian Randomization:** Validated gene-trait associations
using genetic instruments.
- **Protein-Protein Interaction (PPI) Network Analysis:** Explored gene
interaction networks.
- **Drug Repurposing & Molecular Docking:** Screened existing drugs for potential
binding to key targets.
- **Clinical Validation:** Used aldosterone-producing adenoma (APA) tissue samples
to validate gene expression.

SHMT1 is proposed as a promising drug target for PA. The study illustrates how
integrative omics and experimental validation can accelerate target discovery.

Jia, M., Lin, L., Yu, H., & others. (2025). Integrative bioinformatics approach
identifies novel drug targets for hyperaldosteronism, with a focus on SHMT1 as a
promising therapeutic candidate. Scientific Reports, 15, Article 1690.
[DOI](https://doi.org/10.1038/s41598-025-85900-8)

---

## Monthly challenge

**Strobemers** are fuzzy matching seeds that offer better tolerance for mutations
like insertions and deletions compared to traditional k-mers. They're a great
tool for efficient sequence comparison and alignment.

Implement your own **strobemer generator function** in Rust.

- MinStrobe - Choose subsequent strobes by selecting the minimum hash within a
sliding window.
- RandStrobe - Choose subsequent strobes by a pseudo-random but reproducible rule derived from hash values.

**Your function should**:

- Input: DNA string
- Parameters: `k`, `w_min`, and `w_max` (k = strobe length, w = window length)
- Output: a list of strobemers (strings or hashes)

### Bonus Challenge

Invent and implement a **new strobe algorithm**!

Here are a few ideas to inspire you:

- **HybridStrobe** – switch between minstrobe and randstrobe dynamically
- **LoopStrobe** – pick strobes from both forward and reverse directions
- **EntropyStrobe** – prefer high-complexity regions for matching
- **FixedGapStrobe** – always pick the second strobe at a fixed offset

### How to Share

- Post your code as a GitHub repo or Gist
- Share your entry on the discord

---

![Ferris in Bioinformatics](/img/ferris.png)

Have a tool, paper, dataset, or idea you’d like featured?
Have suggestions for the website? Want to submit your answer to the challenge
to potentially be featured on next month’s newsletter?
[![Discord](https://img.shields.io/badge/Join%20Us-Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/dCMfwuze48)

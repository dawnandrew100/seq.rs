+++
title = "Bioinformatics in Rust #1"
date = 2025-07-01

[taxonomies]
tags = ["2025", "July", "newsletter"]
+++

Welcome to the first edition of Bioinformatics in Rust!

The general theme for all the monthly editions will be to have a crate of the month,
a spotlight on a lesser known crate related to bioinformatics,
recent research within bioinformatics,
and a monthly challenge related to one or both of the previously mentioned crates.

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

## Community & Ecosystem Updates

## Research highlights

### 1. Drug Targets for Hyperaldosteronism

**Summary:**

**Key Points:**

Jia, M., Lin, L., Yu, H., & others. (2025). Integrative bioinformatics approach
identifies novel drug targets for hyperaldosteronism, with a focus on SHMT1 as a
promising therapeutic candidate. Scientific Reports, 15, Article 1690.
[DOI](https://doi.org/10.1038/s41598-025-85900-8)

https://www.frontiersin.org/journals/pharmacology/articles/10.3389/fphar.2025.1547131/full
https://www.frontiersin.org/journals/computer-science/articles/10.3389/fcomp.2025.1464122/full
https://www.frontiersin.org/journals/public-health/articles/10.3389/fpubh.2025.1609615/full
https://www.frontiersin.org/journals/molecular-biosciences/articles/10.3389/fmolb.2025.1616073/full

## Dataset of the Month

## Monthly challenge

___

Have a tool, paper, dataset, or idea you’d like featured?  Have suggestions for the website? Want to submit your answer to the challenge to potentially be featured on next month’s newsletter?
[Join the discord](https://discord.gg/dCMfwuze48)!


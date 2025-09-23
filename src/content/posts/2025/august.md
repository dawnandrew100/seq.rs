+++
title = "#2 Natural Language Processing"
date = 2025-08-01

[taxonomies]
tags = ["2025", "August", "newsletter"]
+++

Welcome to the second edition of **Bioinformatics in Rust**!

There was a great reception for the first-ever edition of this newsletter last month!
I hope to keep that momentum going and continue bringing you exciting updates
about Rust and bioinformatics.

---

## Spotlight

### Rust-bert

[crates.io](https://crates.io/crates/rust_bert) |
[docs.rs](https://docs.rs/crate/rust-bert/latest) |
[source](https://github.com/guillaume-be/rust-bert)

Rust-bert is a Rust port of Hugging Face’s
[transformers library](https://github.com/huggingface/transformers).
It offers a wide range of powerful natural language processing (NLP) features,
such as:

- Named Entity Recognition (NER)
- Part-of-Speech (POS) tagging
- Keyword extraction
- Masked Language Modeling
- And more

This, and its extensive suite of tests, makes it a powerful tool for integrating
modern NLP capabilities into a fast, reliable Rust application.

### ttaw

[crates.io](https://crates.io/crates/ttaw) |
[docs.rs](https://docs.rs/ttaw/0.3.0/ttaw/) |
[source](https://github.com/shnewto/ttaw)

Talking to a wall (ttaw) is described by the author as a piecemeal
natural language processing library. The latest version at the time of writing,
v0.3.0, is capable of detecting rhymes, detecting alliteration,
and phonectic transcription.

Functionality:

- Determine if two words rhyme using the Double Metaphone phonetic encoding
- Determine if two words rhyme using CMUdict phonetic encoding
- Determine if two words alliterate using the Double Metaphone phonetic encoding
- Determine if two words alliterate using CMUdict phonetic encoding
- Get the CMUdict phonetic encoding of a word
- Get the Double Metaphone phonetic encoding of a word (port of 
[words/double-metahone](https://github.com/words/double-metaphone) library)

---

## Research Highlights

### Quantum Natural Language Processing

**Summary:**

Natural Language Processing is a subfield of artificial intelligence that aims to
make computers understand human language. Quantum Natural Language Processing
takes this concept and applies it to the realm of quantum computing.
Some of the applications of this within the field of bioinformatics include: detection
of non-coding RNA, the prediction of protein structure and function, biomedical
literature mining, drug discovery/design, and genomic sequence analysis.

Pallavi, G., & Kumar, R.P. (2025).
Quantum natural language processing and its applications in bioinformatics:
a comprehensive review of methodologies, concepts, and future directions.
Frontiers in Computer Science, 7, Article 1464122.
[DOI](https://www.frontiersin.org/journals/computer-science/articles/10.3389/fcomp.2025.1464122/full)

---

## Monthly Challenge

Natural language processing (NLP) consists of many powerful components.
Try programming it on your own!

Some core tasks you can implement include:

- Text Tokenization – Splitting text into smaller units called tokens
(words, phrases, or symbols).
- Word Lemmatization – Reducing words to their base or dictionary form.
- Part-of-Speech Tagging – Assigning grammatical categories
(noun, verb, adjective, etc.) to each token.
- Named Entity Recognition (NER) – Detecting and classifying proper nouns
like people, places, or organizations.
- Coreference Resolution – Identifying when different words refer to the same
entity within a text.

### Bonus Challenge

Combine multiple NLP components into a pipeline that performs more sophisticated
tasks.

#### Example: Grammar Correction Pipeline

Create a system that:

- Tokenizes the input.
- Tags each word with its part of speech.
- Detects grammar issues (e.g., verb tense mismatches, subject-verb disagreement).
- Suggests corrections using lemmatization and rules (or a small ML model).
- Reconstructs the corrected sentence.

### How to Share

- Visit the official
[Challenge GitHub](https://github.com/dawnandrew100/seqrs-challenges) page
- Share your entry on the discord

---

{{ ferris(dir="img/ferris.png", alt="Ferris in Bioinformatics") }}

Have a tool, paper, dataset, or idea you’d like featured?
Have suggestions for the website? Want to submit your answer to the challenge
to potentially be featured on next month’s newsletter?
[![Discord](https://img.shields.io/badge/Join%20Us-Discord-7289DA?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/dCMfwuze48)

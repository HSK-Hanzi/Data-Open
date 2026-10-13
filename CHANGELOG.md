# Changelog

All notable changes to the **HSK Hanzi — Open Data** submodule's bundled corpora are documented in
this file. This submodule holds the openly-licensed property lists bundled into every build of the
app: the CC-CEDICT dictionary, Make Me a Hanzi stroke order, HSK vocabulary, SUBTLEX-CH word
frequencies, per-character readings/etymology/frequency, and the openly-licensed practice-sentence
corpus.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project
adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added

- `HSKVocabulary.plist` records each word's reading in every HSK syllabus that lists it, as
  `syllabusReadings` (standard → lowercase tone-marked letters, in list order), from the HSK 2.0
  lists of clem109/hsk-vocabulary (MIT) and the HSK 3.0 2021 and 2026 lists of krmanik/HSK-3.0
  (Pleco's MIT-licensed transcription of the official syllabi).

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

- `PracticeSentences.plist` holds example sentences for every headword of the three HSK syllabi,
  alongside the sentences it held before, which keep their ids. Each entry records its word
  segmentation as `words` and its level in each HSK standard as `levels` (`old`, `new`, `newest`),
  in place of the single HSK 2.0 `level`; a standard whose syllabus doesn't cover every word in a
  sentence gives it no level. Generated entries also record the `target` word they were written
  for, a `topic`, and, at the lower bands, the `grammar` structure they practice. The file is now a
  binary property list.

- `HSKVocabulary.plist` records each word's reading in every HSK syllabus that lists it, as
  `syllabusReadings` (standard → lowercase tone-marked letters, in list order), from the HSK 2.0
  lists of clem109/hsk-vocabulary (MIT) and the HSK 3.0 2021 and 2026 lists of krmanik/HSK-3.0
  (Pleco's MIT-licensed transcription of the official syllabi).

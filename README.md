# HSK Hanzi — Open Data

Openly-licensed data bundled into the [HSK Hanzi](https://github.com/HSK-Hanzi/iOS) app,
consumed as a git submodule at `Data/Open`. Always bundled, in every build.

## Contents

- `CEDICT.plist` — CC-CEDICT Chinese–English dictionary (CC BY-SA 4.0).
- `HanziStrokeOrder.plist` — Make Me a Hanzi stroke data (LGPL / Arphic PL).
- `HSKVocabulary.plist` — HSK core vocabulary (complete-hsk-vocabulary), with each word's reading in
  the HSK 2.0 and 3.0 syllabi (clem109/hsk-vocabulary, krmanik/HSK-3.0).
- `SUBTLEX-CH-Words.plist` — SUBTLEX-CH word frequencies (Cai & Brysbaert 2010).
- `CharacterReadings.plist`, `CharacterEtymology.plist`, `CharacterFrequency.plist` — per-character
  readings, etymology, and frequency.
- `PracticeSentences.plist` — original practice sentences generated for the app with the Claude API
  (`Tools/generate_sentences.py` in the app repository): example sentences for every HSK
  headword, each with numbered pinyin, an English translation, its word segmentation, and its
  level in each HSK standard.

Each plist uses a self-describing `{ meta, entries }` schema.

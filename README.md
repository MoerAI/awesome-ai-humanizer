# Awesome AI Language [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated, country-by-country guide to open-source **"humanizer" / anti-AI-slop writing skills**: repos that help AI-written text read like natural, native writing in each language.

The list covers the **top 30 AI-using countries** and maps each one to the best-known and best-built repos for its main language(s). Where no credible native-language repo exists, the gap is marked instead of filled with a weak pick.

*Research snapshot: 2026-11-03. Star counts were checked on GitHub that day and will change.*

## Contents

- [Quick start](#quick-start)
- [How the 30 countries were chosen](#how-the-30-countries-were-chosen)
- [Overview table](#overview-table)
- [Country-by-country research](#country-by-country-research)
- [Repos by language](#repos-by-language)
- [Multilingual all-in-one repos](#multilingual-all-in-one-repos)
- [Known gaps](#known-gaps)
- [Other languages worth watching](#other-languages-worth-watching)
- [Caveats](#caveats)
- [Sources](#sources)
- [Contributing](#contributing)

## Quick start

| If you write in... | Start with |
|---|---|
| English | [blader/humanizer](https://github.com/blader/humanizer) |
| Korean | [epoko77-ai/im-not-ai](https://github.com/epoko77-ai/im-not-ai) |
| Simplified Chinese | [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) |
| Traditional Chinese | [kevintsai1202/Humanizer-zh-TW](https://github.com/kevintsai1202/Humanizer-zh-TW) |
| Japanese | [gonta223/humanizer-ja](https://github.com/gonta223/humanizer-ja) |
| German | [marmbiz/humanizer-de](https://github.com/marmbiz/humanizer-de) |
| French / Italian / Swedish | [jurigis/avoid-ai-writing-multilingual](https://github.com/jurigis/avoid-ai-writing-multilingual) |
| Spanish | [peopleworks/SignsofAI](https://github.com/peopleworks/SignsofAI) |
| KO + EN + ZH + JA in one tool | [devswha/patina](https://github.com/devswha/patina) |

**15 repos cover all 30 countries.** The 8 English-speaking countries are all covered by `blader/humanizer`.

## How the 30 countries were chosen

There is no single official ranking of "countries that use AI the most", so two signals were combined:

1. **Adoption rate**: Microsoft AI Economy Institute, *AI Diffusion Report 2026 Q2*. Share of the working-age population (15-64) that used generative AI.
2. **Estimated user volume**: adoption rate x World Bank working-age population (`SP.POP.1564.TO`, 2025).

**Selection rule:** top 15 countries by estimated user volume + the next 15 non-duplicate countries by adoption rate = 30 countries.

- User volumes are **estimates** derived from two sources, not reported figures.
- Taiwan has no World Bank population entry, so its user volume is not computed.
- A web-traffic ranking (e.g. OneLittleWeb) would swap in Bangladesh, Italy, Russia and Turkey. See [Other languages worth watching](#other-languages-worth-watching).

## Overview table

Confidence = my judgement combining popularity with how well the rules, tests and evaluation are documented. **High** / **Medium** / **Low**.

| # | Country | Est. users / adoption | Language(s) | Recommended repo (stars) | Confidence |
|---|---|---|---|---|---|
| 1 | India | 185.3M / 18.5% | English, Hindi | [blader/humanizer](https://github.com/blader/humanizer) (64.1k) · Hindi: gap | High (EN) |
| 2 | China | 171.5M / 17.5% | Simplified Chinese | [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) (21.8k) | High |
| 3 | United States | 72.8M / 33.0% | English | [blader/humanizer](https://github.com/blader/humanizer) | High |
| 4 | Brazil | 29.7M / 20.2% | Brazilian Portuguese | [PedroLLou/humanizador](https://github.com/PedroLLou/humanizador) (0) | Low |
| 5 | Indonesia | 28.8M / 14.8% | Indonesian | [adhiprib/humanizer-indonesia](https://github.com/adhiprib/humanizer-indonesia) (125) | Medium |
| 6 | France | 20.9M / 49.6% | French | [jurigis/avoid-ai-writing-multilingual](https://github.com/jurigis/avoid-ai-writing-multilingual) (19) | Medium |
| 7 | United Kingdom | 19.2M / 43.7% | English | [blader/humanizer](https://github.com/blader/humanizer) | High |
| 8 | Vietnam | 19.2M / 27.9% | Vietnamese | [longhang2004/vietnamese-humanizer](https://github.com/longhang2004/vietnamese-humanizer) (60) | Medium |
| 9 | Mexico | 19.0M / 21.4% | Spanish | [peopleworks/SignsofAI](https://github.com/peopleworks/SignsofAI) (30) | Medium |
| 10 | Pakistan | 18.0M / 11.9% | English, Urdu | [blader/humanizer](https://github.com/blader/humanizer) · Urdu: gap | High (EN) |
| 11 | Japan | 17.9M / 24.7% | Japanese | [gonta223/humanizer-ja](https://github.com/gonta223/humanizer-ja) (161) | Medium |
| 12 | Germany | 16.8M / 32.3% | German | [marmbiz/humanizer-de](https://github.com/marmbiz/humanizer-de) (195) | High |
| 13 | Philippines | 16.2M / 20.7% | English, Filipino | [blader/humanizer](https://github.com/blader/humanizer) · Filipino: gap | High (EN) |
| 14 | Spain | 14.6M / 45.1% | Spanish | [peopleworks/SignsofAI](https://github.com/peopleworks/SignsofAI) | Medium |
| 15 | South Korea | 14.6M / 40.6% | Korean | [epoko77-ai/im-not-ai](https://github.com/epoko77-ai/im-not-ai) (6.4k) | High |
| 16 | UAE | 6.9M / 73.3% | Arabic, English | [OthmanAdi/humanizer-semitic](https://github.com/OthmanAdi/humanizer-semitic) (10) · blader | Medium (AR) |
| 17 | Singapore | 2.9M / 64.3% | English, Chinese | blader · op7418 | High |
| 18 | Ireland | 1.8M / 49.9% | English | [blader/humanizer](https://github.com/blader/humanizer) | High |
| 19 | Norway | 1.8M / 49.4% | Norwegian | [numen-tech/slopornot](https://github.com/numen-tech/slopornot) (58) | Medium |
| 20 | New Zealand | 1.5M / 44.1% | English | [blader/humanizer](https://github.com/blader/humanizer) | High |
| 21 | Netherlands | 5.1M / 43.5% | Dutch | [brunocous/dutch-native](https://github.com/brunocous/dutch-native) (0) | Low |
| 22 | Qatar | 1.1M / 43.5% | Arabic | [OthmanAdi/humanizer-semitic](https://github.com/OthmanAdi/humanizer-semitic) | Medium |
| 23 | Australia | 7.2M / 40.7% | English | [blader/humanizer](https://github.com/blader/humanizer) | High |
| 24 | Belgium | 3.0M / 40.3% | Dutch, French | dutch-native · jurigis | Low-Medium |
| 25 | Switzerland | 2.3M / 39.1% | German, French, Italian | marmbiz · jurigis | High-Medium |
| 26 | Israel | 2.4M / 38.7% | Hebrew | [OthmanAdi/humanizer-semitic](https://github.com/OthmanAdi/humanizer-semitic) | Medium |
| 27 | Canada | 10.4M / 38.5% | English, French | blader · jurigis | High-Medium |
| 28 | Sweden | 2.5M / 37.3% | Swedish | [jurigis/avoid-ai-writing-multilingual](https://github.com/jurigis/avoid-ai-writing-multilingual) | Medium |
| 29 | Austria | 2.1M / 35.4% | German | [marmbiz/humanizer-de](https://github.com/marmbiz/humanizer-de) | High |
| 30 | Taiwan | n/a / 33.8% | Traditional Chinese | [kevintsai1202/Humanizer-zh-TW](https://github.com/kevintsai1202/Humanizer-zh-TW) (935) | High |

Rows 1-15 are the volume group; rows 16-30 are the adoption-rate group.

## Country-by-country research

### Volume group (top 15 by estimated users)

#### 1. India
- **AI use:** ~185.3M estimated users, 18.5% adoption. Largest estimated user base.
- **Languages:** English (business and tech writing), Hindi.
- **Recommended:** [blader/humanizer](https://github.com/blader/humanizer) for English.
- **Hindi:** no credible quality-first repo found. [MrBridgeHQ/human-writer-hi](https://github.com/MrBridgeHQ/human-writer-hi) (0★) has real Hindi rules (danda vs. period, Sanskritized register vs. Hinglish, calques) but is built around beating AI detectors (sub-25% scores), so it is **not recommended**. Fallback: [gencharitaci/humanize-skills](https://github.com/gencharitaci/humanize-skills).

#### 2. China
- **AI use:** ~171.5M estimated users, 17.5% adoption.
- **Language:** Simplified Chinese.
- **Recommended:** [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) (21.8k★, MIT). The most popular non-English humanizer found.
  - Native Chinese rules organized into 31 checks; preserves facts, certainty, voice and genre; treats pattern hits as cues, not automatic edits.
  - Explicitly makes no detector-bypass guarantee.
  - [Test notes](https://github.com/op7418/Humanizer-zh/blob/main/tests/README.md): 18 short cases, a Markdown-structure checker, two long-form comparisons. Self-reported single runs; no cross-model pass rate.

#### 3. United States
- **AI use:** ~72.8M estimated users, 33.0% adoption.
- **Language:** English.
- **Recommended:** [blader/humanizer](https://github.com/blader/humanizer) (64.1k★). The most popular humanizer overall and the template many language ports are based on.
  - Covers chatbot openers, inflated claims, forced rule-of-three lists, repetitive sentence structure and similar patterns, largely based on Wikipedia's *Signs of AI writing*.
  - Voice matching from 2-3 paragraphs of your own writing.
  - Works with Claude Code, Codex and other skill-capable agents.
  - Published a small blind test where reviewers preferred the humanized rewrite 16 out of 16 times. Small sample.

#### 4. Brazil
- **AI use:** ~29.7M estimated users, 20.2% adoption.
- **Language:** Brazilian Portuguese.
- **Recommended (with caution):** [PedroLLou/humanizador](https://github.com/PedroLLou/humanizador) (0★, MIT).
  - 42 patterns in a ~600-line SKILL.md with PT-BR-specific markers. Well-designed rules.
  - The README itself says only 9 of the 42 patterns have direct external evidence; the rest are adapted from the English original.
- **Alternatives:** [finestructure-ai/humanizer-multilingual](https://github.com/finestructure-ai/humanizer-multilingual) (Portuguese file with explicit PT-BR vs. PT-PT handling). For European Portuguese: [mariorabeloneto/evitar-escrita-ia](https://github.com/mariorabeloneto/evitar-escrita-ia) (0★, single commit).

#### 5. Indonesia
- **AI use:** ~28.8M estimated users, 14.8% adoption.
- **Language:** Indonesian.
- **Recommended:** [adhiprib/humanizer-indonesia](https://github.com/adhiprib/humanizer-indonesia) (125★, MIT).
  - Native Indonesian pattern catalog, not a translation: calques, nominalization, repetitive connectors and rhythm, register, paragraph openers.
  - Eight-step draft / audit / revise workflow with a swappable voice preset.
  - `scripts/metrik.py` gives deterministic style metrics calibrated to the author's own corpus. No independent benchmark.
  - Explicitly not for detector evasion.

#### 6. France
- **AI use:** ~20.9M estimated users, 49.6% adoption.
- **Language:** French.
- **Recommended:** [jurigis/avoid-ai-writing-multilingual](https://github.com/jurigis/avoid-ai-writing-multilingual) (19★, MIT).
  - [SKILL-FR.md](https://github.com/jurigis/avoid-ai-writing-multilingual/blob/main/SKILL-FR.md): 45 French-specific patterns with P0-P2 severity, tiered vocabulary, context/tolerance profiles, rewrite and detect-only modes, self-check.
  - Patterns are grounded in cited sources per language. No executable output tests.
  - Same repo covers German, Italian, Romanian and Swedish.

#### 7. United Kingdom
- **AI use:** ~19.2M estimated users, 43.7% adoption.
- **Language:** English.
- **Recommended:** [blader/humanizer](https://github.com/blader/humanizer). Use the voice-matching feature with a British-English sample to keep spelling and tone.

#### 8. Vietnam
- **AI use:** ~19.2M estimated users, 27.9% adoption.
- **Language:** Vietnamese.
- **Recommended:** [longhang2004/vietnamese-humanizer](https://github.com/longhang2004/vietnamese-humanizer) (60★, MIT).
  - Four skills including a Vietnamese humanizer and a translationese cleaner. Rules grouped into lexical, structural, discourse and pragmatic tells.
  - Prefers light edits and can return `no_change` or flag for author review.
  - [Evaluation methodology](https://github.com/longhang2004/vietnamese-humanizer/blob/main/docs/evaluation-methodology.md): 44 patterns, 103 examples, 70 benchmark cases. Cases are agent-authored; no independent baseline.

#### 9. Mexico
- **AI use:** ~19.0M estimated users, 21.4% adoption.
- **Language:** Spanish.
- **Recommended:** [peopleworks/SignsofAI](https://github.com/peopleworks/SignsofAI) (30★, MIT).
  - Native Spanish JSON rule pack plus an explainable linter and an agent skill.
  - README claims calibration against 296 pre-2022 human texts to limit false positives. That is false-positive calibration, not a rewrite-quality benchmark.
  - The skill deliberately avoids giving a numeric "AI score".

#### 10. Pakistan
- **AI use:** ~18.0M estimated users, 11.9% adoption.
- **Languages:** English, Urdu.
- **Recommended:** [blader/humanizer](https://github.com/blader/humanizer) for English.
- **Urdu:** no credible dedicated repo found, and the multilingual repos do not cover it. Marked as a gap.

#### 11. Japan
- **AI use:** ~17.9M estimated users, 24.7% adoption.
- **Language:** Japanese.
- **Recommended:** [gonta223/humanizer-ja](https://github.com/gonta223/humanizer-ja) (161★). The most popular Japanese-specific repo found. Built around a 20-pattern checklist; no public tests.
- **Alternatives:**
  - [devswha/patina](https://github.com/devswha/patina) (382★): KO/EN/ZH/JA in one tool with optional meaning-preservation checks.
  - [geonwoo-jeong/japanese-humanizer](https://github.com/geonwoo-jeong/japanese-humanizer) (4★, MIT): careful Japanese rules (translationese, nominalization, connectors, register mixing; P1-P3 priorities; protects facts, negation and technical terms). Small but well-designed.

#### 12. Germany
- **AI use:** ~16.8M estimated users, 32.3% adoption.
- **Language:** German.
- **Recommended:** [marmbiz/humanizer-de](https://github.com/marmbiz/humanizer-de) (195★, MIT). The strongest European-language repo found.
  - [72-rule German catalog](https://github.com/marmbiz/humanizer-de/blob/main/references/patterns.md), 19 of them backed by a linter.
  - Test corpus and coverage matrix.
  - German only. Not a detector or detector-bypass tool.

#### 13. Philippines
- **AI use:** ~16.2M estimated users, 20.7% adoption.
- **Languages:** English, Filipino.
- **Recommended:** [blader/humanizer](https://github.com/blader/humanizer) for English.
- **Filipino / Tagalog:** no credible dedicated repo found. Marked as a gap.

#### 14. Spain
- **AI use:** ~14.6M estimated users, 45.1% adoption.
- **Language:** Spanish.
- **Recommended:** [peopleworks/SignsofAI](https://github.com/peopleworks/SignsofAI). See Mexico.
- **Alternative:** [finestructure-ai/humanizer-multilingual](https://github.com/finestructure-ai/humanizer-multilingual) Spanish file.

#### 15. South Korea
- **AI use:** ~14.6M estimated users, 40.6% adoption.
- **Language:** Korean.
- **Recommended:** [epoko77-ai/im-not-ai](https://github.com/epoko77-ai/im-not-ai) (6.4k★).
  - Covers translationese (`~를 통해`, `~에 있어서`, double passives, heavy nominalization), mechanical lists, stock conclusions and over-emphasis.
  - Preserves original tone, genre, facts, numbers, proper nouns and claim strength.
  - Over-editing guard: warns above 30% change and stops above 50%.
  - Supports Claude Code, Codex, Copilot CLI and Gemini CLI (the Gemini version is reduced).
  - Has check scripts and regression tests. Public evaluation is mostly the author's own.
- **Alternatives:**
  - [NomaDamas/k-skill](https://github.com/NomaDamas/k-skill) (8.2k★ for the whole 133-skill bundle): includes `korean-humanizer`, rebuilt on im-not-ai's method, with voice matching and length targeting.
  - [DaleSeo/korean-skills](https://github.com/DaleSeo/korean-skills) (248★): 40-pattern humanizer chained with grammar and style-consistency checks. Good for technical and business docs.
  - [hjongc/humanizer-kr](https://github.com/hjongc/humanizer-kr) (20★): focuses on over-polite honorifics, chatbot-style flow, product copy and notices.
  - [devswha/patina](https://github.com/devswha/patina) (382★).

### Adoption-rate group (next 15 by share of population using AI)

#### 16. United Arab Emirates
- **AI use:** 73.3% adoption, the highest in the world (~6.9M estimated users).
- **Languages:** Arabic, English.
- **Recommended:** [OthmanAdi/humanizer-semitic](https://github.com/OthmanAdi/humanizer-semitic) (10★, MIT) for Arabic; [blader/humanizer](https://github.com/blader/humanizer) for English.
  - Separate skills for Modern Standard Arabic (28 patterns), Egyptian (25), Levantine (25) and Hebrew (35).
  - **No Gulf-dialect version**, so MSA is the closest fit for the UAE.
  - Only a few commits; no test or eval suite found.

#### 17. Singapore
- **AI use:** 64.3% adoption, second highest (~2.9M estimated users).
- **Languages:** English, Chinese.
- **Recommended:** [blader/humanizer](https://github.com/blader/humanizer) + [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh).

#### 18. Ireland
- **AI use:** 49.9% adoption (~1.8M estimated users).
- **Language:** English.
- **Recommended:** [blader/humanizer](https://github.com/blader/humanizer).

#### 19. Norway
- **AI use:** 49.4% adoption (~1.8M estimated users).
- **Language:** Norwegian (Bokmål, Nynorsk).
- **Recommended:** [numen-tech/slopornot](https://github.com/numen-tech/slopornot) (58★, MIT).
  - Supports English, Spanish, German, Italian, Swedish, Danish and Norwegian Bokmål. Nynorsk gets AI-tell checks only.
  - Localized lexical categories plus shared structural rules; LIX readability for Bokmål.
  - Word lists are described as empirical, not sourced. No output eval suite.

#### 20. New Zealand
- **AI use:** 44.1% adoption (~1.5M estimated users).
- **Language:** English.
- **Recommended:** [blader/humanizer](https://github.com/blader/humanizer).

#### 21. Netherlands
- **AI use:** 43.5% adoption (~5.1M estimated users).
- **Language:** Dutch.
- **Recommended (with caution):** [brunocous/dutch-native](https://github.com/brunocous/dutch-native) (0★, CC BY 4.0).
  - Targets translationese and structural defects in Dutch (particles, *er*, modal verbs, word order, calques) with BE/NL variant handling.
  - Deterministic grep linter plus eval cases and CI.
  - Test cases have not yet been run, so no pass rate is published. More a "write native Dutch" skill than a humanizer.

#### 22. Qatar
- **AI use:** 43.5% adoption (~1.1M estimated users).
- **Language:** Arabic.
- **Recommended:** [OthmanAdi/humanizer-semitic](https://github.com/OthmanAdi/humanizer-semitic) (MSA skill). Same Gulf-dialect caveat as the UAE.

#### 23. Australia
- **AI use:** 40.7% adoption (~7.2M estimated users).
- **Language:** English.
- **Recommended:** [blader/humanizer](https://github.com/blader/humanizer).

#### 24. Belgium
- **AI use:** 40.3% adoption (~3.0M estimated users).
- **Languages:** Dutch (Flemish), French.
- **Recommended:** [brunocous/dutch-native](https://github.com/brunocous/dutch-native) (explicit Belgian-Dutch variant handling) + [jurigis/avoid-ai-writing-multilingual](https://github.com/jurigis/avoid-ai-writing-multilingual) for French.

#### 25. Switzerland
- **AI use:** 39.1% adoption (~2.3M estimated users).
- **Languages:** German, French, Italian.
- **Recommended:** [marmbiz/humanizer-de](https://github.com/marmbiz/humanizer-de) for German; [jurigis/avoid-ai-writing-multilingual](https://github.com/jurigis/avoid-ai-writing-multilingual) for French and Italian ([SKILL-IT.md](https://github.com/jurigis/avoid-ai-writing-multilingual/blob/main/SKILL-IT.md): 42 patterns with a second-pass audit).

#### 26. Israel
- **AI use:** 38.7% adoption (~2.4M estimated users).
- **Language:** Hebrew.
- **Recommended:** [OthmanAdi/humanizer-semitic](https://github.com/OthmanAdi/humanizer-semitic). Hebrew skill has 35 patterns covering construct state, gender agreement, binyanim and register.

#### 27. Canada
- **AI use:** 38.5% adoption (~10.4M estimated users).
- **Languages:** English, French.
- **Recommended:** [blader/humanizer](https://github.com/blader/humanizer) + [jurigis/avoid-ai-writing-multilingual](https://github.com/jurigis/avoid-ai-writing-multilingual). The French rules target France French, so check Québécois usage manually.

#### 28. Sweden
- **AI use:** 37.3% adoption (~2.5M estimated users).
- **Language:** Swedish.
- **Recommended:** [jurigis/avoid-ai-writing-multilingual](https://github.com/jurigis/avoid-ai-writing-multilingual). SKILL-SV has 42 Swedish-specific patterns with P0-P2 severity, before/after examples and context tolerance. Best-documented Swedish option found.
- **Alternative:** [numen-tech/slopornot](https://github.com/numen-tech/slopornot) Swedish catalog.

#### 29. Austria
- **AI use:** 35.4% adoption (~2.1M estimated users).
- **Language:** German.
- **Recommended:** [marmbiz/humanizer-de](https://github.com/marmbiz/humanizer-de).

#### 30. Taiwan
- **AI use:** 33.8% adoption. User volume not computed (no World Bank population entry).
- **Language:** Traditional Chinese.
- **Recommended:** [kevintsai1202/Humanizer-zh-TW](https://github.com/kevintsai1202/Humanizer-zh-TW) (935★, MIT).
  - Traditional Chinese adaptation of the revised Humanizer-zh rules. Preserves information, voice, register and protected file structures.
  - Separates prose humanization from invisible-character watermark cleanup.
  - 18 editing cases plus a structure-preservation script. Human-checked single runs; no cross-model pass rate.

## Repos by language

| Language | Repo | Stars | License | Countries |
|---|---|---|---|---|
| English | [blader/humanizer](https://github.com/blader/humanizer) | 64.1k | see repo | IN, US, UK, PK, PH, AE, SG, IE, NZ, AU, CA |
| Simplified Chinese | [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) | 21.8k | MIT | CN, SG |
| Korean | [epoko77-ai/im-not-ai](https://github.com/epoko77-ai/im-not-ai) | 6.4k | see repo | KR |
| Traditional Chinese | [kevintsai1202/Humanizer-zh-TW](https://github.com/kevintsai1202/Humanizer-zh-TW) | 935 | MIT | TW |
| German | [marmbiz/humanizer-de](https://github.com/marmbiz/humanizer-de) | 195 | MIT | DE, AT, CH |
| Japanese | [gonta223/humanizer-ja](https://github.com/gonta223/humanizer-ja) | 161 | see repo | JP |
| Indonesian | [adhiprib/humanizer-indonesia](https://github.com/adhiprib/humanizer-indonesia) | 125 | MIT | ID |
| Vietnamese | [longhang2004/vietnamese-humanizer](https://github.com/longhang2004/vietnamese-humanizer) | 60 | MIT | VN |
| Norwegian | [numen-tech/slopornot](https://github.com/numen-tech/slopornot) | 58 | MIT | NO |
| Spanish | [peopleworks/SignsofAI](https://github.com/peopleworks/SignsofAI) | 30 | MIT | MX, ES |
| French, Italian, Swedish | [jurigis/avoid-ai-writing-multilingual](https://github.com/jurigis/avoid-ai-writing-multilingual) | 19 | MIT | FR, BE, CH, CA, SE |
| Arabic, Hebrew | [OthmanAdi/humanizer-semitic](https://github.com/OthmanAdi/humanizer-semitic) | 10 | MIT | AE, QA, IL |
| Brazilian Portuguese | [PedroLLou/humanizador](https://github.com/PedroLLou/humanizador) | 0 | MIT | BR |
| Dutch | [brunocous/dutch-native](https://github.com/brunocous/dutch-native) | 0 | CC BY 4.0 | NL, BE |
| KO / EN / ZH / JA | [devswha/patina](https://github.com/devswha/patina) | 382 | MIT | KR, JP, CN, US (alt.) |

## Multilingual all-in-one repos

No single repo is both popular **and** verified across many languages yet. The best options:

- **[devswha/patina](https://github.com/devswha/patina)** (382★, MIT): Korean, English, Chinese, Japanese in one CLI. Deterministic offline analysis (`patina inspect`, `patina-score`) plus LLM-backed rewriting (Claude, Codex or Gemini CLI, or an API key). Optional `--verify` with number/claim checks and meaning-preservation floors. States it is for permitted AI-assisted drafting, not detector evasion.
- **[gencharitaci/humanize-skills](https://github.com/gencharitaci/humanize-skills)** (7★, CC BY 4.0): 20 languages in one skill (shared rules + per-language files such as `ko.md`, `ja.md`, `zh.md`, plus tone/use-case rules; detects the input language). The author says examples were model-written and not native-reviewed; spot checks of the Korean example found added content not in the source. Good structure, not yet verified quality. No Hindi, Urdu or Filipino.
- **[finestructure-ai/humanizer-multilingual](https://github.com/finestructure-ai/humanizer-multilingual)** (3★, MIT): 10 languages (JA, ZH, ES, PT, FR, DE, IT, HE, AR, RU), with a manual AI/counter-sample corpus. No Korean or Dutch. The repo itself points to marmbiz (German) and jurigis for deeper coverage.

## Known gaps

| Language | Countries affected | Status |
|---|---|---|
| Hindi | India | Only a detector-evasion-oriented repo ([MrBridgeHQ/human-writer-hi](https://github.com/MrBridgeHQ/human-writer-hi), 0★). Not recommended. |
| Urdu | Pakistan | No credible repo found. |
| Filipino / Tagalog | Philippines | No credible repo found. |
| Gulf Arabic | UAE, Qatar | Only MSA / Egyptian / Levantine skills exist. |
| Québécois French | Canada | No dedicated rules. |

Contributions for these languages are especially welcome.

## Other languages worth watching

These countries appear in web-traffic rankings (e.g. Bangladesh, Italy, Russia, Turkey, Poland) but not in the 30 above.

| Language | Repo | Notes |
|---|---|---|
| Russian | [ilyautov/humanizer-ru](https://github.com/ilyautov/humanizer-ru) (~408★, MIT) | 67-rule native catalog; scanner calibrated on tens of thousands of texts, but the AI-vs-human eval is small and uses older models. |
| Turkish | [oguzhankayan/turkish-native](https://github.com/oguzhankayan/turkish-native) (~89★, MIT) | 57 rules, 105 regression cases including positive controls. Pre-1.0; closer to "natural Turkish" localization. |
| Italian | [jurigis/avoid-ai-writing-multilingual](https://github.com/jurigis/avoid-ai-writing-multilingual) | 42 Italian patterns. |
| Finnish | [Hakku/finnish-humanizer](https://github.com/Hakku/finnish-humanizer) (21★, MIT) | 27 rules (12 Finnish-specific). Tests cover packaging only. |
| Polish | [pielas-activy/humanizer-pl](https://github.com/pielas-activy/humanizer-pl) (9★, MIT) | Small eval set. |
| Bengali | none found | Gap (Bangladesh). |

## Caveats

- **Stars measure popularity, not quality.** "Recommended" weighs popularity together with how well rules, tests and evaluations are documented. It is not a head-to-head benchmark; these tools were not run on the same input.
- **None of these guarantees passing AI detectors**, and this list is not meant for academic dishonesty. The goal is clearer, more natural writing.
- **Country ≠ language.** Countries are mapped to their main written languages; regional variants (PT-BR vs. PT-PT, Gulf Arabic, Québécois French) may be only partly covered.
- User volumes are modeled estimates, not reported numbers.

## Sources

- Microsoft AI Economy Institute, [AI Diffusion Report 2026 Q2](https://www.microsoft.com/en-us/research/wp-content/uploads/2026/09/Microsoft-AI-Diffusion-Report-2026-Q2.pdf) and [data CSV](https://github.com/microsoft/ai-diffusion-report/blob/main/data/AI_Diffusion_Q22026_Update.csv)
- Microsoft On the Issues, [The continued state of global AI diffusion in 2026](https://blogs.microsoft.com/on-the-issues/2026/09/21/the-continued-state-of-global-ai-diffusion-in-2026/)
- World Bank, [Population ages 15-64, total (SP.POP.1564.TO)](https://data.worldbank.org/indicator/SP.POP.1564.TO)
- OneLittleWeb, [AI Tools country traffic dashboard](https://onelittleweb.com/digital-market-intelligence/ai-tools/) (used only for the "worth watching" list)
- Wikipedia, [Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)
- Each repo's README, SKILL/rule files and test docs, linked above.

## Contributing

PRs welcome, especially for the [known gaps](#known-gaps). When adding a repo, please include:

1. Language and countries it serves
2. Star count and the date you checked it
3. What the rules actually cover (not just the README pitch)
4. Whether it has tests or an evaluation, and their limits

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this list.

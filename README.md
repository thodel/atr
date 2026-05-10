# Automated Text Recognition — Teaching Resource

[![GitHub Pages](https://img.shields.io/badge/site-thodel.github.io%2Fatr-blue)](https://thodel.github.io/atr/)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

A Quarto-based teaching resource on Automated Text Recognition (OCR/HTR) for historical documents. Published at **[thodel.github.io/atr](https://thodel.github.io/atr/)**.

## Contents

| Section | Description |
|---|---|
| [Introduction](content/introduction/index.qmd) | OCR vs. HTR, the recognition pipeline, CER/WER, transcription policies |
| [eScriptorium](content/escriptorium/index.qmd) | Open-source platform built on Kraken: workflow, training, export |
| [Open-Source Models](content/models/open-source/index.qmd) | Curated overview of Kraken/eScriptorium models (CATMuS, TRIDIS, BiblIA, …) |
| [HTR-United](content/models/htr-united/index.qmd) | Community standard for sharing HTR datasets and models |
| [TrOCR](content/modern-approaches/trocr/index.qmd) | Microsoft's transformer-based OCR model |
| [Vision Language Models](content/modern-approaches/vlms/index.qmd) | GPT-4o, Gemini, Llama, and other VLMs applied to HTR |
| [Quiz](content/quiz/index.qmd) | Kahoot-style 12-question self-test |
| [Literature](content/literature/index.qmd) | Live bibliography from Zotero group 4971878 |

## Local Preview

Requires [Quarto](https://quarto.org/docs/get-started/) ≥ 1.5.

```bash
quarto preview
```

The site renders to `_site/` on build.

## Structure

This site is built with [Quarto](https://quarto.org/) following the same conventions as [dhbern.github.io](https://dhbern.github.io/), making it straightforward to integrate into that site later.

```
_quarto.yml          # Quarto project config (nav, theme, site-url)
_brand.yml           # Brand colors and typography
custom.scss          # SCSS overrides
styles.css           # CSS (Switzer font, quiz styles, Zotero styles)
index.qmd            # Homepage
content/
  introduction/      # What is ATR?
  escriptorium/      # eScriptorium platform
  models/
    open-source/     # Kraken/eScriptorium model catalogue
    htr-united/      # HTR-United standard
  modern-approaches/
    trocr/           # TrOCR
    vlms/            # Vision Language Models
  quiz/              # Interactive quiz
  literature/        # Zotero bibliography
.github/workflows/
  quarto-publish.yml # Render + deploy to GitHub Pages on push to main
```

## License

- **Content:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- **Code:** [AGPL-3.0](https://www.gnu.org/licenses/agpl-3.0.html)

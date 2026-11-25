# KSAVS 2026, Software Component Provenance Identification

[![English](https://ysl-ryudo.github.io/assets/diagrams/language-en-current.svg)](README.md) [![한국어](https://ysl-ryudo.github.io/assets/diagrams/language-ko.svg)](README.ko.md) [![日本語](https://ysl-ryudo.github.io/assets/diagrams/language-ja.svg)](README.ja.md)

**First author, oral presenter**

[45th Fall Conference of the Korea Software Assessment and Valuation Society](https://ksavs.or.kr/board/board.asp?Action=content&B_CATE=BBS2&GotoPage=1&b_code=33)

5 ~ 7 Nov 2026, Hotel Whistle Lark, Jeju, Korea. Oral presentation on 6 Nov 2026, Session IV: Software Forensics and Assessment I.

## A Comparative Analysis of Software Component Provenance Identification Techniques

Compared CENTRIS, BinaryAI, LibAM, BinCoFer and BLADE through their inputs, matching evidence and outputs. Analyzed how shared dependencies, partial reuse and missing references limit source attribution.

Organized the comparison around reference coverage, matched locations, alternative explanations and unresolved questions. Component detection, reuse locations and direct provenance require different evidence.

[Paper (PDF)](paper/ksavs-2026-paper.pdf), [Portfolio](https://ysl-ryudo.github.io/en/research/ksavs/)

## Comparison framework

| Technique | Evidence and output | Interpretation |
| --- | --- | --- |
| CENTRIS | Separates borrowed code before comparing source functions. | Observed project history is not proof of first authorship. |
| BinaryAI | Matches binary functions to source functions using embeddings and structural context. | Small reuse fragments and shared dependencies can affect detection. |
| LibAM | Matches similar functions and call-graph regions. | A reused region does not by itself identify an exact version. |
| BinCoFer | Refines function features and aggregates weighted similarity. | Shared functions can leave original provenance unresolved. |
| BLADE | Retrieves candidates and verifies multiple structured evidence sources. | Results depend on available evidence and model reliability. |

This paper compares five published techniques through a literature analysis. It does not report a new algorithm or a head-to-head benchmark.

## Authors

Young-Sang Lee, Jung-Min Park, Geon Park, Myeong-Jae Lee, MD Shariful Islam, Nguyễn Hữu Nhật Minh, Hye-Young Kim

## Related research

[ICEA 2026, MOD provenance reconstruction](https://github.com/YSL-RyuDo/icea-2026-mod-provenance-research), [WISA 2026, game image verification](https://github.com/YSL-RyuDo/wisa-2026-game-asset-verification), [CISC-W 2025, game pricing](https://github.com/YSL-RyuDo/cisc-w-2025-game-economy)

# KSAVS 2026, Software Component Provenance Identification

[![English](https://ysl-ryudo.github.io/assets/diagrams/language-en.svg)](README.md) [![한국어](https://ysl-ryudo.github.io/assets/diagrams/language-ko.svg)](README.ko.md) [![日本語](https://ysl-ryudo.github.io/assets/diagrams/language-ja-current.svg)](README.ja.md)

**筆頭著者、口頭発表**

[韓国ソフトウェア鑑定評価学会 第45回秋季学術大会](https://ksavs.or.kr/board/board.asp?Action=content&B_CATE=BBS2&GotoPage=1&b_code=33)

2026.11.05 ~ 07, 韓国・済州、Hotel Whistle Lark. 2026.11.06 口頭発表、Session IV: Software Forensics and Assessment I。

## ソフトウェア構成要素の出所識別手法に関する比較分析

CENTRIS、BinaryAI、LibAM、BinCoFer、BLADEの入力資料、判断根拠、出力を比較しました。共通依存関係、部分的な再利用、参照資料の欠落が出所識別に与える影響を分析しました。

参照範囲、対応箇所、代替説明、未確定事項の四項目で比較を整理しました。構成要素の検出、再利用箇所の特定、直接の再利用関係の判断に必要な根拠を区別しました。

[論文 (PDF)](paper/ksavs-2026-paper.pdf), [Portfolio](https://ysl-ryudo.github.io/ja/research/ksavs/)

## 手法の比較

| 手法 | 根拠と出力 | 解釈上の限界 |
| --- | --- | --- |
| CENTRIS | 借用コードを分離してソース関数の再利用を比較します。 | 観測された履歴と実際の初回作成は区別する必要があります。 |
| BinaryAI | 埋め込みと構造的な文脈からバイナリとソースの関数を対応付けます。 | 少量の再利用と共通依存関係が検出結果に影響します。 |
| LibAM | 類似関数とコールグラフ領域を比較します。 | 再利用領域の検出と正確なバージョン識別は別の問題です。 |
| BinCoFer | 関数特徴を精製し、重み付き類似度を集計します。 | 共通関数の最初の出所が未確定となる場合があります。 |
| BLADE | 候補を検索し、構造化した複数の証拠を検証します。 | 利用可能な証拠とモデルの信頼性に依存します。 |

公開された五つの手法を対象とした文献比較です。新たなアルゴリズムや同一条件での性能比較実験を提案した研究ではありません。

## 共著者

Young-Sang Lee, Jung-Min Park, Geon Park, Myeong-Jae Lee, MD Shariful Islam, Nguyễn Hữu Nhật Minh, Hye-Young Kim

## 関連研究

[ICEA 2026, MOD provenance reconstruction](https://github.com/YSL-RyuDo/ICEA2026ModProvenanceResearch), [WISA 2026, game image verification](https://github.com/YSL-RyuDo/WISA2026GameAssetVerification), [CISC W 2025, game pricing](https://github.com/YSL-RyuDo/CISCW2025GameEconomy)

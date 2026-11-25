# KSAVS 2026, Software Component Provenance Identification

[![English](https://ysl-ryudo.github.io/assets/diagrams/language-en.svg)](README.md) [![한국어](https://ysl-ryudo.github.io/assets/diagrams/language-ko-current.svg)](README.ko.md) [![日本語](https://ysl-ryudo.github.io/assets/diagrams/language-ja.svg)](README.ja.md)

**제1저자, 구두 발표**

[한국소프트웨어감정평가학회 제45회 추계학술대회](https://ksavs.or.kr/board/board.asp?Action=content&B_CATE=BBS2&GotoPage=1&b_code=33)

2026.11.05 ~ 07, 제주 휘슬락호텔. 2026.11.06 구두 발표, Session IV: 소프트웨어 포렌식 및 감정 I.

## 소프트웨어 구성요소 출처 식별 기법에 대한 비교분석

CENTRIS, BinaryAI, LibAM, BinCoFer, BLADE의 입력 자료, 판단 근거와 출력을 비교했습니다. 공통 의존성, 부분 재사용, 참조 자료 누락이 출처 식별에 미치는 영향을 분석했습니다.

참조 범위, 대응 위치, 대안 설명, 미확정 사항의 네 항목으로 비교를 정리했습니다. 구성요소 탐지, 재사용 위치 확인, 직접 재사용 관계의 판단에 필요한 근거를 구분했습니다.

[논문 (PDF)](paper/ksavs-2026-paper.pdf), [Portfolio](https://ysl-ryudo.github.io/ko/research/ksavs/)

## 기법별 비교

| 기법 | 판단 근거와 출력 | 해석할 때의 한계 |
| --- | --- | --- |
| CENTRIS | 차용 코드를 분리한 뒤 소스 함수의 재사용을 비교합니다. | 관측된 프로젝트 이력과 실제 최초 작성은 구분해야 합니다. |
| BinaryAI | 임베딩과 구조적 맥락으로 바이너리와 소스 함수를 대응시킵니다. | 적은 재사용량과 공통 의존성이 탐지 결과에 영향을 줍니다. |
| LibAM | 유사 함수와 호출 그래프 영역을 함께 비교합니다. | 재사용 영역의 탐지와 정확한 버전 식별은 별도 문제입니다. |
| BinCoFer | 함수 특징을 정제하고 가중 유사도를 집계합니다. | 공통 함수의 최초 출처가 미확정으로 남을 수 있습니다. |
| BLADE | 후보를 검색한 뒤 구조화한 여러 증거를 검증합니다. | 사용 가능한 증거와 모델의 신뢰도에 영향을 받습니다. |

공개된 다섯 기법을 대상으로 한 문헌 비교분석입니다. 새로운 알고리즘이나 동일 조건의 성능 비교 실험을 제안한 연구는 아닙니다.

## 공동저자

Young-Sang Lee, Jung-Min Park, Geon Park, Myeong-Jae Lee, MD Shariful Islam, Nguyễn Hữu Nhật Minh, Hye-Young Kim

## 관련 연구

[ICEA 2026, MOD provenance reconstruction](https://github.com/YSL-RyuDo/ICEA2026ModProvenanceResearch), [WISA 2026, game image verification](https://github.com/YSL-RyuDo/WISA2026GameAssetVerification), [CISC W 2025, game pricing](https://github.com/YSL-RyuDo/CISCW2025GameEconomy)

[README.md](https://github.com/user-attachments/files/32741930/README.md)
# CME September Trading Challenge 2026

## English

### Overview

This repository documents my participation in the **CME Group Trading Challenge – September 2026**, a simulated futures trading competition using a **$25,000 virtual account**. The available trading universe included CME futures across equity indices, energy, FX, rates, metals, agriculture, and micro contracts.

The project focuses less on the final P&L itself and more on the **decision-making process, event-driven market analysis, position sizing, risk management, and post-trade review** developed during the competition.

### Trading Approach

My main framework was event-driven and macro-oriented:

**Market expectations → Event / catalyst → Surprise assessment → Factor confirmation → Price confirmation → Entry / sizing → Exit → Post-trade review**

For central-bank events, the key principle was to avoid trading the headline in isolation. Instead, I focused on the difference between market expectations and the actual policy path, then looked for confirmation from relevant market factors before considering execution.

A specific pre-event framework was prepared for the **Bank of England decision**, linking:

**BoE policy path → UK 2Y rates → GBP confirmation → Pullback execution**

The executed trade log itself was concentrated in:

- **CLV26** — WTI Crude Oil futures
- **MNQZ26** — Micro E-mini Nasdaq-100 futures

GBP futures were part of the event-driven preparation process, but no closed GBP futures trade appears in the final trade log.

### Risk Management

The competition highlighted the importance of measuring risk in **dollar terms rather than contract count alone**.

Examples from the review:

- Normal event risk budget: **$100–$125**
- Higher-conviction setup: **$175–$190 maximum**
- No first-spike chasing
- No averaging down
- Avoid duplicate exposure to the same underlying factor
- Use smaller contracts when possible for more precise position sizing

One of the main lessons was that a single futures contract can still represent materially different risk depending on the contract multiplier and stop distance.

### Performance Summary

| Metric | Result |
|---|---:|
| Starting Virtual Capital | $25,000 |
| Closed Episodes | 25 |
| Net P&L | -$63 |
| Win Rate | 60.0% |
| Profit Factor | 0.95 |
| Max Drawdown | $710 |
| Average Win | $86 |
| Average Loss | -$135.3 |
| Largest Win | $440 |
| Largest Loss | -$500 |

Performance differed substantially by instrument:

| Instrument | Closed Episodes | Net P&L |
|---|---:|---:|
| CLV26 | 4 | -$550 |
| MNQZ26 | 21 | +$487 |

The final **-$63** therefore masks a clear instrument-level split. Early losses in crude oil drove most of the drawdown, while later MNQ execution recovered a large portion of those losses.

### Key Takeaways

The competition reinforced several practical lessons:

1. **Win rate is not enough.**  
   A 60% win rate did not produce a positive result because the average loss exceeded the average win.

2. **Instrument selection matters.**  
   CL and MNQ produced very different outcomes, making instrument-level attribution more informative than aggregate P&L alone.

3. **Risk should be normalized across contracts.**  
   Contract count is not a sufficient measure of exposure when futures have different multipliers and tick values.

4. **Confirmation is more useful than prediction in event-driven trading.**  
   For macro events, I found it more useful to define confirmation rules across rates, FX, and price action than to rely only on a directional forecast.

5. **Trade logging needs to capture process, not only fills.**  
   Future logs should preserve **Thesis / Factor / Entry / Stop / Size / Exit Reason** for each trade so that post-trade attribution is more rigorous.

### Reports

- [English Review](./CME_September_Trading_Challenge_2026_Review_EN.pdf)
- [Korean Review](./CME_September_Trading_Challenge_2026_Review_KR.pdf)

The reports include the competition overview, market context, strategy framework, risk management rules, daily trading record, performance analysis, trade case studies, and final review.

---

## 한국어

### 개요

이 저장소는 **CME Group Trading Challenge – September 2026** 참가 과정과 사후 분석을 정리한 프로젝트입니다. 대회는 **가상자금 $25,000**으로 진행되었으며, 주가지수, 에너지, FX, 금리, 금속, 농산물 및 마이크로 계약을 포함한 CME 선물 상품을 거래할 수 있었습니다.

이 프로젝트의 핵심은 최종 손익 자체보다, 대회 기간 동안 적용하고 수정한 **의사결정 프로세스, 이벤트 드리븐 시장 분석, 포지션 사이징, 리스크 관리, 사후 리뷰**를 체계적으로 기록하는 데 있습니다.

### 거래 접근법

기본적인 프레임워크는 다음과 같습니다.

**시장 기대 → 이벤트 / 촉매 → 서프라이즈 판단 → 팩터 확인 → 가격 확인 → 진입 / 사이징 → 청산 → 사후 리뷰**

중앙은행 이벤트에서는 헤드라인만 보고 방향을 예측하기보다, **시장 기대와 실제 정책 경로의 차이**를 먼저 판단하고 관련 팩터가 같은 방향을 확인할 때만 실행 후보로 보는 방식을 사용했습니다.

특히 영란은행 이벤트 전에는 다음과 같은 구조를 준비했습니다.

**BoE 정책 경로 → UK 2Y 금리 → GBP 확인 → Pullback 실행**

실제 체결 로그는 다음 두 상품에 집중되었습니다.

- **CLV26** — WTI Crude Oil 선물
- **MNQZ26** — Micro E-mini Nasdaq-100 선물

GBP 선물은 이벤트 드리븐 플레이북의 후보였지만, 최종 로그에는 GBP 선물의 종료 거래가 기록되어 있지 않습니다.

### 리스크 관리

이번 대회에서 가장 중요하게 확인한 점 중 하나는 **계약 수보다 달러 기준 위험을 직접 관리해야 한다는 점**이었습니다.

사전에 설정한 원칙은 다음과 같습니다.

- 일반 이벤트 리스크: **$100–$125**
- 확신도가 높은 A+ 셋업: **최대 $175–$190**
- 첫 스파이크 추격 금지
- 물타기 금지
- 동일 팩터에 대한 중복 노출 지양
- 가능하면 더 작은 계약을 활용해 세밀하게 포지션 사이징

실제 거래를 통해 같은 1계약이라도 상품별 multiplier와 stop distance에 따라 달러 손실이 크게 달라질 수 있다는 점을 확인했습니다.

### 성과 요약

| 지표 | 결과 |
|---|---:|
| 시작 가상자금 | $25,000 |
| 종료 에피소드 | 25 |
| 순손익 | -$63 |
| 승률 | 60.0% |
| Profit Factor | 0.95 |
| 최대 낙폭 | $710 |
| 평균 이익 | $86 |
| 평균 손실 | -$135.3 |
| 최대 이익 | $440 |
| 최대 손실 | -$500 |

상품별 성과는 뚜렷하게 달랐습니다.

| 상품 | 종료 에피소드 | 순손익 |
|---|---:|---:|
| CLV26 | 4 | -$550 |
| MNQZ26 | 21 | +$487 |

따라서 최종 **-$63**만으로는 대회 전체의 성과 구조를 설명하기 어렵습니다. 초기 CL 손실이 최대 낙폭의 대부분을 만들었고, 이후 MNQ 거래에서 상당 부분을 회복했습니다.

### 핵심 교훈

1. **승률만으로는 성과를 판단할 수 없다.**  
   승률은 60%였지만 평균 손실이 평균 이익보다 커 최종 손익은 플러스로 연결되지 않았습니다.

2. **상품 선택 자체가 성과에 큰 영향을 준다.**  
   CL과 MNQ의 성과 차이가 컸기 때문에 전체 손익보다 상품별 attribution이 더 유용했습니다.

3. **선물 리스크는 계약 수가 아니라 공통 달러 기준으로 비교해야 한다.**  
   multiplier와 tick value가 다르기 때문에 단순 계약 수만으로 위험을 비교하면 왜곡될 수 있습니다.

4. **이벤트 드리븐 거래에서는 예측보다 confirmation rule이 중요하다.**  
   거시 이벤트에서는 한 방향을 미리 맞히는 것보다 금리, FX, 가격 움직임이 같은 해석을 확인하는지 점검하는 방식이 더 유용했습니다.

5. **거래 로그에는 체결뿐 아니라 의사결정 과정도 남겨야 한다.**  
   향후에는 모든 거래에 대해 **Thesis / Factor / Entry / Stop / Size / Exit Reason**을 함께 기록해 사후 분석의 정확도를 높일 계획입니다.

### 상세 리포트

- [English Review](./CME_September_Trading_Challenge_2026_Review_EN.pdf)
- [Korean Review](./CME_September_Trading_Challenge_2026_Review_KR.pdf)

리포트에는 대회 개요, 시장 환경, 전략 구조, 리스크 관리, 일자별 거래 기록, 성과 분석, 거래 사례 및 실패 분석, 최종 리뷰가 포함되어 있습니다.

---

> **Note:** This repository documents a simulated trading competition for educational and portfolio purposes. It is not investment advice.

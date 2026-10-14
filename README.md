# CME September Trading Challenge 2026

## English

### Overview

This repository documents my participation in the **CME Group Trading Challenge – September 2026**, a simulated futures trading competition using a **$25,000 virtual account**. The tradable universe included CME futures across equity indices, energy, FX, rates, metals, agriculture, and micro contracts.

The project focuses on the **decision process, macro-event analysis, position sizing, risk management, and post-trade review** developed during the competition.

### Strategy classification

The most accurate description of the approach is **discretionary, macro-event-aware intraday futures trading**.

- Scheduled releases and central-bank decisions were treated as **catalysts and context** for a trade, not as stand-alone signals.
- Entries required discretionary interpretation of expectations, cross-market signals, and price action.
- This was not a systematic or algorithmic strategy.
- In institutional investment terminology, **event-driven** usually refers to special situations such as merger arbitrage, spin-offs, restructurings, tender offers, or other security-specific corporate events. That label is therefore not used here for the overall strategy.

### Decision framework

**Market expectations → Scheduled macro catalyst → Surprise assessment → Cross-market confirmation → Price confirmation → Entry / sizing → Exit → Post-trade review**

For central-bank decisions, the principle was to avoid trading the headline in isolation. I first assessed the gap between market expectations and the communicated policy path, then looked for confirmation from the relevant rates, FX, and price signals before considering execution.

A specific pre-event playbook was prepared for the **Bank of England decision**:

**BoE policy path → UK 2Y yield response → GBP confirmation → Pullback entry**

The closed trade log itself was concentrated in:

- **CLV26** — WTI Crude Oil futures
- **MNQZ26** — Micro E-mini Nasdaq-100 futures

GBP futures were included in the pre-event research, but no closed GBP futures trade appears in the final trade log. The playbook should therefore be read as preparation rather than executed performance.

### Risk management

The competition highlighted the importance of measuring risk in **dollars rather than contract count alone**.

- Normal per-trade risk budget: **$100–$125**
- Higher-conviction setup: **$175–$190 maximum**
- No first-spike chasing
- No averaging down
- Avoid duplicate exposure to the same underlying risk driver
- Use smaller contracts where possible for more precise position sizing

One futures contract can represent materially different risk across instruments because multipliers, tick values, volatility, and stop distances differ.

### Performance summary

| Metric | Result |
|---|---:|
| Starting Virtual Capital | $25,000 |
| Closed Trade Episodes | 25 |
| Net P&L | -$63 |
| Win Rate | 60.0% |
| Profit Factor | 0.95 |
| Max Drawdown | $710 |
| Average Win | $86 |
| Average Loss | -$135.3 |
| Largest Win | $440 |
| Largest Loss | -$500 |

Performance differed substantially by instrument:

| Instrument | Closed Trade Episodes | Net P&L |
|---|---:|---:|
| CLV26 | 4 | -$550 |
| MNQZ26 | 21 | +$487 |

The final **-$63** therefore masks a clear instrument-level split. Early losses in crude oil drove most of the drawdown, while later MNQ execution recovered a large portion of those losses.

### Key takeaways

1. **Win rate is not enough.** A 60% win rate did not produce a positive result because the average loss exceeded the average win.
2. **Instrument selection matters.** CL and MNQ produced very different outcomes, so instrument-level attribution is more informative than aggregate P&L alone.
3. **Risk should be normalized across contracts.** Contract count is not a sufficient exposure measure when multipliers and tick values differ.
4. **For macro-event trading, confirmation was more useful than prediction.** Cross-market confirmation rules across rates, FX, and price action were more useful than relying only on a directional forecast.
5. **Trade logs should capture the process, not only fills.** Future logs should preserve **Thesis / Catalyst / Cross-market signals / Entry / Stop / Size / Exit reason** for each trade.

### Files

- [English review](./CME%20SeptemberTrading%20Challenge/CME_September_Trading_Challenge_2026_Review_EN.pdf)
- [Korean review](./CME%20SeptemberTrading%20Challenge/CME_September_Trading_Challenge_2026_Review_KR_v3.pdf)
- [Trade log](./CME%20SeptemberTrading%20Challenge/challenge_trade_log.csv)

The reports include the competition overview, market context, decision framework, risk rules, daily record, performance analysis, case studies, and final review.

---

## 한국어

### 개요

이 저장소는 **CME Group Trading Challenge – September 2026** 참가 과정과 사후 분석을 정리한 프로젝트입니다. 대회는 **가상자금 $25,000**으로 진행되었으며, 주가지수, 에너지, FX, 금리, 금속, 농산물 및 마이크로 계약을 포함한 CME 선물을 거래할 수 있었습니다.

이 프로젝트는 최종 손익뿐 아니라 대회 기간에 적용하고 수정한 **의사결정 과정, 거시 이벤트 분석, 포지션 사이징, 리스크 관리, 거래 복기**를 기록하는 데 목적이 있습니다.

### 전략 분류

이 접근법은 **거시 이벤트를 반영한 재량적 장중 선물 거래(discretionary, macro-event-aware intraday futures trading)**로 설명하는 것이 가장 정확합니다.

- 경제지표 발표와 중앙은행 결정은 단독 매매 신호가 아니라 **촉매와 시장 맥락**으로 사용했습니다.
- 시장 기대, 교차시장 신호, 가격 움직임을 재량적으로 해석한 뒤 진입했습니다.
- 체계적·알고리즘 매매 전략은 아닙니다.
- 기관투자 업계에서 **이벤트 드리븐(event-driven)**은 일반적으로 합병 차익거래, 분할, 구조조정, 공개매수 등 기업별 특수상황 전략을 뜻합니다. 혼동을 피하기 위해 이 프로젝트 전체를 이벤트 드리븐 전략이라고 부르지 않습니다.

### 의사결정 프레임워크

**시장 기대 → 예정된 거시 촉매 → 서프라이즈 판단 → 교차시장 확인 → 가격 확인 → 진입 / 사이징 → 청산 → 사후 리뷰**

중앙은행 결정에서는 헤드라인만 보고 거래하지 않았습니다. 시장 기대와 실제 정책 경로의 차이를 먼저 판단한 뒤, 관련 금리·FX·가격 신호가 같은 해석을 지지할 때 실행 후보로 보았습니다.

영란은행 결정 전에는 다음 플레이북을 준비했습니다.

**BoE 정책 경로 → 영국 2년물 금리 반응 → GBP 확인 → 되돌림 진입**

종료된 실제 거래 로그는 다음 두 상품에 집중되었습니다.

- **CLV26** — WTI Crude Oil 선물
- **MNQZ26** — Micro E-mini Nasdaq-100 선물

GBP 선물은 사전 이벤트 분석에 포함됐지만 최종 로그에는 종료된 GBP 거래가 없습니다. 따라서 해당 플레이북은 실현 성과가 아니라 사전 준비 과정으로 해석해야 합니다.

### 리스크 관리

이번 대회에서 확인한 핵심 원칙은 **계약 수가 아니라 달러 기준 위험을 직접 관리하는 것**이었습니다.

- 일반 거래당 리스크 예산: **$100–$125**
- 확신도가 높은 셋업: **최대 $175–$190**
- 첫 급등락 추격 금지
- 물타기 금지
- 동일한 기초 위험요인에 대한 중복 노출 지양
- 가능한 경우 더 작은 계약으로 세밀하게 사이징

같은 1계약이라도 상품별 승수, 틱 가치, 변동성, 손절 폭에 따라 실제 달러 위험은 크게 달라질 수 있습니다.

### 성과 요약

| 지표 | 결과 |
|---|---:|
| 시작 가상자금 | $25,000 |
| 종료 거래 에피소드 | 25 |
| 순손익 | -$63 |
| 승률 | 60.0% |
| Profit Factor | 0.95 |
| 최대 낙폭 | $710 |
| 평균 이익 | $86 |
| 평균 손실 | -$135.3 |
| 최대 이익 | $440 |
| 최대 손실 | -$500 |

| 상품 | 종료 거래 에피소드 | 순손익 |
|---|---:|---:|
| CLV26 | 4 | -$550 |
| MNQZ26 | 21 | +$487 |

최종 **-$63**만으로는 성과 구조를 충분히 설명하기 어렵습니다. 초기 CL 손실이 낙폭 대부분을 만들었고, 이후 MNQ 거래에서 상당 부분을 회복했습니다.

### 핵심 교훈

1. **승률만으로는 성과를 판단할 수 없습니다.** 승률은 60%였지만 평균 손실이 평균 이익보다 컸습니다.
2. **상품 선택 자체가 성과에 큰 영향을 줍니다.** 전체 손익뿐 아니라 상품별 성과기여 분석이 필요합니다.
3. **선물 리스크는 공통 달러 기준으로 비교해야 합니다.** 승수와 틱 가치가 다른 상품을 계약 수만으로 비교하면 위험이 왜곡됩니다.
4. **거시 이벤트 거래에서는 예측보다 확인이 더 유용했습니다.** 금리·FX·가격 움직임이 같은 해석을 지지하는지 확인하는 규칙이 방향 예측만 하는 것보다 유용했습니다.
5. **거래 로그에는 체결뿐 아니라 의사결정 과정도 남겨야 합니다.** 향후에는 **투자논리 / 촉매 / 교차시장 신호 / 진입 / 손절 / 규모 / 청산 사유**를 함께 기록할 계획입니다.

### 파일

- [영문 리뷰](./CME%20SeptemberTrading%20Challenge/CME_September_Trading_Challenge_2026_Review_EN.pdf)
- [국문 리뷰](./CME%20SeptemberTrading%20Challenge/CME_September_Trading_Challenge_2026_Review_KR_v3.pdf)
- [거래 로그](./CME%20SeptemberTrading%20Challenge/challenge_trade_log.csv)

리뷰에는 대회 개요, 시장 환경, 의사결정 구조, 리스크 관리, 일자별 거래 기록, 성과 분석, 사례 및 최종 복기가 포함되어 있습니다.

---

> This repository documents a simulated trading competition for educational and portfolio purposes. It is not investment advice.



---
layout: single
title: "6.Buried Pipe Corrosion"
categories: Piping
tag: [Corrosion, buried, SSC]
toc: true
---

# 지중배관 부식과 **Cathodic Protection** 완전 가이드

> 배관이 땅속에 묻히는 순간, 토양·전해질·외부 전류·미생물 등 수많은 변수가 “보이지 않는 곳”에서 부식을 일으킵니다.  
> **코팅 + Cathodic Protection(CP)**의 다중 방어 체계를 설계·시공·운영 전 주기에 걸쳐 유지해야 파이프라인의 수명과 안전성을 확보할 수 있습니다.

---

## 1. 지중배관 외부 부식 메커니즘

| 주요 메커니즘           | 핵심 원인                        | 특징 & 사례                                                  |
| ----------------------- | -------------------------------- | ------------------------------------------------------------ |
| **균일·차등산소전지**   | 토양 내 산소 농도 차             | 피복 손상 부위가 양극 → 금속 용해                            |
| **갈바닉 부식**         | 이종 금속 전위 차                | 용접부, 연결플랜지 등 국부 손상 심화                         |
| **국부(크리브·핀홀)**   | 토양 수분·염분 불균일            | 빠른 벽 두께 감소, 핀홀 생성                                 |
| **MIC** *(SRB, APB 등)* | 미생물 부산물(H₂S·산성)          | 음극 반응 촉진, 국부 가속 부식 :contentReference[oaicite:0]{index=0} |
| **Stray DC 전류**       | 전철 궤도·DC 설비 누설           | 전류 반출점 집중 손상                                        |
| **AC 부식**             | 송전선·HVDC 인접                 | 코팅 결함점에서 높은 AC 전류밀도 → 급격한 금속 용출 :contentReference[oaicite:1]{index=1} |
| **SCC / n-pH SCC**      | 응력 + 수분 + 중성~약알칼리 토양 | 균열 성장, 파괴 사고 사례 다수                               |

> **토양 저항률(ρ) < 2 kΩ·cm**, **수분·염분 ↑** 환경일수록 각종 부식 메커니즘이 가속됩니다.

---

## 2. 토양·환경 인자 체크리스트

- **토양 저항률**(Soil resistivity)  
- **수분/배수 조건** & 지하수위  
- **pH / 염이온(Cl⁻·SO₄²⁻)** 농도  
- **온도** & 유기물 함량(→ MIC)  
- **외부 전기장**(철도·송전선 인접)  
- **설계·시공 품질**(코팅 결함율, 절연이음 상태)

---

## 3. 1차 방어선: **외부 절연코팅**

| 코팅 시스템                   | 특징                    | 대표 적용                |
| ----------------------------- | ----------------------- | ------------------------ |
| **FBE**                       | 전기저항 ↑, 굴곡성 보통 | 장거리 가스관            |
| **3-Layer PE/PP**             | 충격·인장 강도 우수     | 토질 변화 구간, 고기계력 |
| **Heat-shrink Sleeve / Tape** | 현장 보수 용이          | 분기라인·피팅            |

> 설계 기준(NACE SP0169): **코팅 결함율 ≤ 1 %, 절연저항 ≥ 10⁹ Ω·m²** :contentReference[oaicite:2]{index=2}

---

## 4. 2차 방어선: **Cathodic Protection (CP)**

### 4-1. 원리 한눈에 보기
- 전기화학 반응에서 **배관을 음극**(환원)으로 만들어 **산화(철 용해) 반응**을 억제  
- 두 가지 방식  
  1. **희생양극(Sacrificial Anode)**: Mg·Zn·Al 합금이 “더 쉽게” 산화 → 배관 보호  
  2. **외부전원(ICCP)**: 정류기에서 전류 공급 → 토양 저항률·배관 길이 큰 경우 적합

### 4-2. 보호 전위 기준

| 기준                                | 설명                                                         |
| ----------------------------------- | ------------------------------------------------------------ |
| **-850 mV (Cu/CuSO₄, Instant-OFF)** | 국제적으로 가장 널리 적용되는 철강 배관 보호 기준 :contentReference[oaicite:3]{index=3} |
| **100 mV Polarization**             | CP 인가 전·후 100 mV 이상 전위 이동 시 보호로 간주           |
| **Net Protective Current**          | 배관-토양 계면에 순환 보호 전류 확인                         |

> 최신 NACE SP0169-2024와 ISO 15589-1(육상 파이프라인 CP)에서 위 기준을 채택·보완 중 :contentReference[oaicite:4]{index=4}

### 4-3. 설계 핵심 포인트  
1. **전류 요구량 계산**: (코팅 결함 면적 × 설계 전류밀도)  
2. **양극/그라운드베드 배치**: 토양 ρ, 배관 형상 고려 → 균일 전위 분포 확보  
3. **과보호 방지**: -1200 mV 이하에서는 수소 취성·코팅 박리 위험 ↑  
4. **절연이음(IJF)**: CP 구역 분리, Stray 전류 차단  
5. **AC/Stray DC 완화**: 접지 케이블, 드레이닝 와이어, 감쇄 리액터 등 적용 :contentReference[oaicite:5]{index=5}

### 4-4. 모니터링 & 유지관리

| 방법                                       | 목적                              | 주기          |
| ------------------------------------------ | --------------------------------- | ------------- |
| **CIPS (Close Interval Potential Survey)** | 전위 연속 프로파일 → CP 음영 확인 | 1 년          |
| **DCVG / ACVG**                            | 코팅 결함 위치·심각도 정량        | 2–3 년        |
| **ER Probe / 쿠폰**                        | 금속 손실률(mm/y) 실측            | 6 개월        |
| **Rectifier Log & 원격 모니터링**          | 전류·전압 이상 탐지               | 월간 / 실시간 |

---

## 5. 설계-시공-운영 **Lifecycle** 체크포인트

1. **설계**: 토양·환경 조사 → 코팅 시스템 + CP 타입 선정  
2. **시공**: Holiday Tester로 100 % 코팅 결함 검증 → 양극·절연이음 설치  
3. **시운전**: Initial Depolarization Test → 보호전위 달성 확인  
4. **운영**: 정기 CIPS/DCVG·피그 검사 → 결함 위치 보수 → CP 전류 재조정  
5. **폐기·교체**: 잔존 수명 평가(RLA/RBI) → 교체 시기도 CP 로그로 추적

---

## 6. 국제 표준 & 가이드 한눈에

| 표준               | 최근판 | 주요 내용                                                    |
| ------------------ | ------ | ------------------------------------------------------------ |
| **NACE SP0169**    | 2024   | 토양 배관 CP 설계·운영 전체 지침                             |
| **ISO 15589-1**    | 2015   | 육상 파이프라인 CP 설계 요구사항                             |
| **NACE SP21424**   | 2018   | AC 부식 위험 평가·완화 :contentReference[oaicite:6]{index=6} |
| **EN 12954**       | 2023   | CP 시스템 성능 기준                                          |
| **API RP 1169**    | 2020   | 건설 단계 품질·무결성 관리                                   |
| **AWWA C214/C215** | 2022   | 스틸관 열수축·분체코팅 시공                                  |

---

## 7. 결론 & 현업 팁

- **“코팅이 1차, CP가 2차”**라는 원칙을 명심하세요. 코팅 품질이 좋을수록 CP 전류 요구량은 기하급수적으로 감소합니다.  
- **온·오프라인 모니터링**을 병행해 “보이지 않는 부식”을 데이터로 관리해야 합니다.  
- 설계 단계에서 **AC/Stray 전류 평가**를 놓치면, 운영 단계에서 뒤늦게 리스크와 비용이 폭증합니다.  
- 마지막으로, 토양·환경 조건은 **프로젝트 현장마다 다르기** 때문에, 국제 표준(ISO·NACE)을 기본 틀로 삼고 **현장 실측 데이터**로 세부 값을 보정하는 것이 관건입니다.

---

> 🎯 **다중 방어(코팅 → CP → 모니터링) 전략**을 꾸준히 유지하면, 30 년 이상 무사고 파이프라인 운영도 가능합니다. 당신의 파이프라인이 “눈에 보이지 않는” 위험으로부터 자유롭길 바랍니다!

---

### 참고 문헌

- NACE International, **SP0169-2024** *“Control of External Corrosion on Underground or Submerged Metallic Piping Systems”* :contentReference[oaicite:7]{index=7}  
- ISO 15589-1:2015, *“Cathodic Protection of Pipeline Systems – Part 1: Buried Pipelines”* :contentReference[oaicite:8]{index=8}  
- NACE SP21424-2018, *“AC Induced Corrosion on Cathodically Protected Pipelines”* :contentReference[oaicite:9]{index=9}  
- Technical Toolboxes, *“AC Corrosion on Buried Pipelines”* (Blog, 2023) :contentReference[oaicite:10]{index=10}  
- AUCSC, *“Criteria for Cathodic Protection”* (Course Text, 2024) :contentReference[oaicite:11]{index=11}  
- V&A Engineering, *“CP Testing Methods for Pipelines”* (Blog, 2022) :contentReference[oaicite:12]{index=12}  
# 포트폴리오 프로젝트 마스터 가이드

> **GitHub:** sth00619/data_projects  
> **기간:** 2026-04-06 ~ 2026-06-30 (85일, 12주)  
> **목표:** 8개 프로젝트 완성 + GitHub 매일 커밋 + 면접 대비

---

## 1. 프로젝트 목록 및 상태

| # | 프로젝트명 | 분류 | 핵심 스택 | 목표 완료 | 상태 |
|---|-----------|------|----------|----------|------|
| P1 | 실시간 금융 거래 이상탐지 대시보드 | 데이터 (소형) | XGBoost, Airflow, FastAPI, Redis | W2 (4/19) | ⬜ 미시작 |
| P2 | SaaS 고객 이탈 예측 및 코호트 분석 | 데이터 (소형) | LightGBM, SHAP, dbt, Spring Boot | W4 (5/3) | ⬜ 미시작 |
| P3 | 서울 대중교통 지연 예측 및 경로 최적화 | 데이터 (공간) | PostGIS, TimescaleDB, LSTM, Mapbox | W6 (5/17) | ⬜ 미시작 |
| P4 | K-뷰티 글로벌 트렌드 분석 및 수요 예측 | 데이터 (API/NLP) | pytrends, PRAW, ES, Prophet, Spring Boot | W10 (6/14) | ⬜ 미시작 |
| P5 | 서울 상권 분석 및 점포 입지 추천 | 데이터 (공간) | H3, PostGIS, Deck.gl, GWR, LightGBM | W9 (6/7) | ⬜ 미시작 |
| P6 | 글로벌 지역·산업 인텔리전스 플랫폼 | 지구본 (대형) | Mapbox Globe, Deck.gl, 10종 API, PostGIS | W12 (6/28) | ⬜ 미시작 |
| P7M | 이커머스 그로스 마케팅 성과 분석 플랫폼 | 마케팅 | GA4, RFM, CRM, ROAS, FastAPI | W7 (5/24) | ⬜ 미시작 |
| P7P | SaaS 프로덕트 분석 및 기능 개선 플랫폼 | PM | Aha Moment, RICE, dbt, Spring Boot | W8 (5/31) | ⬜ 미시작 |

---

## 2. 12주 작업 일정

### Phase 1 · 기초 파이프라인 완성 (4/6 ~ 4/19)

| 주차 | 날짜 | 작업 내용 |
|------|------|----------|
| W1 | 4/6 ~ 4/12 | **P1** 데이터셋 확보 + EDA + DB 스키마 설계 + SQL 쿼리 |
| W2 | 4/13 ~ 4/19 | **P1** ML 모델링 + FastAPI + 시각화 + README ✅ |

### Phase 2 · 코호트 + 포트폴리오 뼈대 (4/20 ~ 5/3)

| 주차 | 날짜 | 작업 내용 |
|------|------|----------|
| W3 | 4/20 ~ 4/26 | **P2** 데이터셋 + EDA + Star Schema + dbt 세팅 / **포트폴리오 사이트** Next.js 뼈대 |
| W4 | 4/27 ~ 5/3 | **P2** LightGBM + SHAP + Spring Boot + 코호트 히트맵 + README ✅ |

### Phase 3 · 공간 DB + 마케팅·PM (5/4 ~ 5/24)

| 주차 | 날짜 | 작업 내용 |
|------|------|----------|
| W5 | 5/4 ~ 5/10 | **P3** 공공API 수집 + PostGIS 스키마 + TimescaleDB + 공간 쿼리 |
| W6 | 5/11 ~ 5/17 | **P3** LSTM + Mapbox + README ✅ / **P7M** GA4 + 퍼널 + ROAS + CRM 시작 |
| W7 | 5/18 ~ 5/24 | **P7M** A/B 테스트 + FastAPI + 시각화 + README ✅ / **P7P** Faker + Aha Moment + dbt |

### Phase 4 · 공간 분석 심화 + NLP (5/25 ~ 6/7)

| 주차 | 날짜 | 작업 내용 |
|------|------|----------|
| W8 | 5/25 ~ 5/31 | **P7P** Spring Boot + A/B 테스트 + RICE + README ✅ / **P5** H3 격자 + PostGIS + ML |
| W9 | 6/1 ~ 6/7 | **P5** Deck.gl + SHAP + README ✅ / **P4** pytrends + PRAW + ES + Prophet |

### Phase 5 · P4 마무리 + P6 지구본 (6/8 ~ 6/28)

| 주차 | 날짜 | 작업 내용 |
|------|------|----------|
| W10 | 6/8 ~ 6/14 | **P4** Spring Boot + README ✅ / **P6** 10종 API 수집 + DB 스키마 + PostGIS |
| W11 | 6/15 ~ 6/21 | **P6** ML 클러스터링 + Mapbox Globe + Deck.gl 레이어 구현 |
| W12 | 6/22 ~ 6/28 | **P6** ArcLayer + H3Layer + 상세 패널 + FastAPI + README ✅ / 포트폴리오 사이트 전체 연결 + 배포 |

> **버퍼:** 6/29 ~ 6/30 — 최종 배포 점검, 링크 확인, README 오탈자 수정

---

## 3. 매 프로젝트 진행 단계 (요청 형식)

Claude에게 작업을 요청할 때 아래 형식으로 말하면 해당 단계를 바로 진행합니다.

```
"P1 1단계 — 데이터셋 확보"
"P3 3단계 — ML 모델링 코드 구현"
"P6 2단계 — 라이브러리 매핑"
```

### 1단계 | 데이터셋 확보
- 정확한 다운로드 URL (Kaggle / 공공API / 오픈 데이터)
- 실제 row 수, 컬럼 목록, 라이센스 확인
- 로컬 저장 경로 및 Git LFS 처리 여부
- 데이터 한계 및 주의사항 명시

### 2단계 | 라이브러리 + 역량 매핑
- 사용 라이브러리 목록 + 선택 이유 (왜 이 라이브러리인가, 대안과 트레이드오프)
- 해당 프로젝트가 커버하는 자격증/부트캠프 범위 명시
  - ADsP: 어느 분석 기법 해당하는지
  - SQLD: 어느 SQL 기능 활용하는지
  - 부트캠프: 몇 주차 커리큘럼과 매핑되는지
- 면접에서 "왜 이 기술을 선택했나?" 답변 초안

### 3단계 | 코드 구현
아래 순서로 실행 가능한 코드를 제공합니다.

```
EDA 노트북 → DB 스키마 SQL → 파이프라인(Airflow/Prefect) → ML/분석 → API(FastAPI/Spring Boot)
```

- 각 코드 블록 상단에 **"직접 작성 권장"** / **"Claude Code 활용 가능"** 구분 표시
- 직접 작성 권장: 분석 로직, 임계값 선정, A/B 테스트 해석, 모델 평가 기준
- Claude Code 활용: Airflow DAG 보일러플레이트, Docker Compose, Spring Boot 스캐폴딩

### 4단계 | 시각화 + 문서화
- GitHub README 초안 (문제 정의 → 가설 → 파이프라인 → 인사이트 → 한계)
- 핵심 시각화 코드 (Recharts / D3.js / Deck.gl / Mapbox)
- 면접 대비 질문 3개 + 답변 초안

---

## 4. 면접 대비 — 매 프로젝트마다 정리할 3가지

### 4-1. AI를 언제 쓰고 안 쓰는지

각 프로젝트 README에 **"개발 방식"** 섹션을 추가합니다.

```markdown
## 개발 방식

| 구분 | 작업 내용 |
|------|----------|
| 직접 작성 | 임계값 선정 로직, A/B 테스트 통계 해석, 모델 평가 기준, 분석 인사이트 도출 |
| Claude Code 활용 | Airflow DAG 보일러플레이트, Docker Compose, Spring Boot 엔드포인트 스캐폴딩 |
```

면접 질문 예시: *"AI 도구를 어떻게 활용하나요?"*
→ "파이프라인 보일러플레이트는 Claude Code로 빠르게 잡고, 분석 판단이 필요한 임계값 설정·모델 선택·인사이트 도출은 직접 작성합니다. 코드가 왜 그렇게 작동하는지 설명할 수 없는 부분은 사용하지 않습니다."

### 4-2. 문제의식 / 주제의식

각 프로젝트를 시작하기 전 비즈니스 언어로 한 문단 정리합니다.

| 프로젝트 | 문제의식 핵심 |
|---------|-------------|
| P1 Fraud | 이커머스/핀테크에서 사기 거래로 인한 차지백 비용 증가 → 규칙 기반 탐지의 낮은 재현율 문제 |
| P2 Churn | SaaS 월간 이탈률 증가 → 이탈 위험 고객을 조기 식별해 리텐션 캠페인 설계 필요 |
| P3 Transit | 서울 출퇴근 지연 불편 → 공공데이터 기반 예측으로 최적 경로 추천 가능성 |
| P4 K-Beauty | K-뷰티 해외 시장 진출 시 국가별 타이밍 의사결정 데이터 부재 |
| P5 Location | 소상공인 점포 출점 시 주관적 판단 의존 → 객관적 데이터 기반 입지 추천 |
| P6 Globe | 한국 기업 해외 진출 시 다차원 지표 통합 분석 도구 부재 |
| P7M Marketing | 마케팅 예산 증가에도 ROAS 하락 → 채널별 성과 차이와 CRM 전략 최적화 필요 |
| P7P PM | SaaS 무료→유료 전환율 낮음 → 온보딩 병목 진단과 Aha Moment 발굴 필요 |

### 4-3. 스킬·라이브러리·개념 숙지

코드 구현 전에 Claude가 개념 질문을 던집니다. 답변을 정리한 뒤 코드로 넘어갑니다.

예시 질문:
- "SHAP 값이 뭔지 한 문장으로 설명해보세요"
- "윈도우 함수 LAG()가 이 프로젝트에서 왜 필요한지 설명해보세요"
- "Isolation Forest와 XGBoost의 차이를 비지도/지도 관점에서 설명해보세요"
- "Star Schema에서 Fact 테이블과 Dimension 테이블의 역할 차이는?"
- "MAPE와 RMSE 중 시계열 예측 평가에 뭘 쓸지, 왜?"

---

## 5. 자격증 범위 매핑 (프로젝트별 커버리지)

### ADsP 범위 → 프로젝트 매핑

| ADsP 기법 | 해당 프로젝트 | 구체적 구현 |
|----------|-------------|-----------|
| 분류분석 | P1, P2, P6 | XGBoost, LightGBM, Random Forest |
| 군집분석 | P2, P5, P6 | K-Means, DBSCAN |
| 시계열 분석 | P3, P4 | LSTM, Prophet, SARIMAX |
| 연관분석 | P4, P6 | Apriori 알고리즘 |
| 가설검정 | P1, P2, P7M, P7P | z-test, Bayesian, 카이제곱 |
| 회귀분석 | P3, P5 | LightGBM 회귀, GWR |

### SQLD 범위 → 프로젝트 매핑

| SQLD 주제 | 해당 프로젝트 | 구체적 구현 |
|----------|-------------|-----------|
| 윈도우함수 (LAG, RANK, FIRST_VALUE) | P1, P2, P5, P7M | 거래 패턴 피처, 리텐션 계산 |
| GROUPING SETS / ROLLUP / CUBE | P1, P7M | 다차원 집계 |
| 정규화 (3NF, BCNF) | 전 프로젝트 | DB 스키마 설계 문서화 |
| Materialized View | P2, P5, P7P | 격자별 피처, 온보딩 퍼널 집계 |
| 복합 인덱스 / 실행계획 | P3, P5 | PostGIS GIST 인덱스, B-tree |
| CTE | P2, P7M, P7P | 코호트, 퍼널, Aha Moment 쿼리 |

---

## 6. 기술 스택 전체 목록

### 공통 인프라

```
Python 3.11+          pandas, NumPy, scikit-learn
PostgreSQL 16         PostGIS 3.4, TimescaleDB
Docker Compose        모든 프로젝트 컨테이너화
GitHub Actions        CI/CD (lint + test)
Next.js 14            포트폴리오 사이트 + 각 프로젝트 프론트엔드
```

### 프로젝트별 추가 스택

| 프로젝트 | 추가 스택 |
|---------|----------|
| P1 | XGBoost, imbalanced-learn, FastAPI, Redis, Airflow, Recharts |
| P2 | LightGBM, SHAP, lifelines, pymc, dbt, Spring Boot, D3.js |
| P3 | GeoPandas, TimescaleDB, TensorFlow/Keras, Mapbox GL JS |
| P4 | pytrends, PRAW, spaCy, KoNLPy, Elasticsearch, Prophet, statsmodels |
| P5 | h3-py, GWR (mgwr), Deck.gl H3HexagonLayer, GeoAlchemy2 |
| P6 | Mapbox GL JS v3 (globe), Deck.gl (ArcLayer, IconLayer, BitmapLayer), Nivo |
| P7M | GA4 BigQuery Public Dataset, Faker, scipy, Recharts |
| P7P | Faker, dbt, statsmodels (power analysis), D3.js Sankey |

---

## 7. GitHub 커밋 원칙

```
매일 최소 1 커밋 (EDA 노트북, SQL 스크립트, README 초안도 커밋 대상)
```

### 커밋 메시지 형식

```
[P1] feat: add XGBoost fraud detection model
[P2] data: add telco churn dataset EDA notebook
[P3] sql: add PostGIS spatial schema with GIST index
[P6] viz: integrate Deck.gl ArcLayer for trade flow
[SITE] feat: add P1 project card to portfolio main
```

### 브랜치 전략

```
main          완성된 프로젝트만 머지
dev/p1        P1 작업 브랜치
dev/p2        P2 작업 브랜치
...
dev/site      포트폴리오 사이트 작업 브랜치
```

---

## 8. 위험 구간 및 대응 방안

| 위험 구간 | 위험 내용 | 대응 방안 |
|----------|----------|----------|
| W6 (5/11~5/17) | P3 LSTM 디버깅 + P7M 동시 시작 | P3 LSTM은 LightGBM으로 먼저 완성 후 LSTM은 보완 |
| W9 (6/1~6/7) | P4 다중 API 수집 불안정 | pytrends rate limit 대비 로컬 캐싱 먼저 구현 |
| W10~W12 (6/8~6/28) | P6 Mapbox Globe + Deck.gl 통합 난이도 | W9 중 미니 POC (지구본 기본 회전만) 30분 선행 |
| 전 기간 | 공공 API 서비스 불안정 | 백업 데이터셋 (Kaggle 대체) 항상 준비 |

---

## 9. 포트폴리오 사이트 구조

```
song-data.dev/                    메인 (8개 프로젝트 카드)
├── /fraud                        P1 라이브 대시보드
├── /churn                        P2 코호트 플랫폼
├── /transit                      P3 지도 대시보드
├── /kbeauty                      P4 트렌드 분석
├── /location                     P5 입지 추천 지도
├── /geoindustry                  P6 3D 지구본
├── /marketing                    P7M 그로스 마케팅
└── /product                      P7P PM 대시보드
```

---

## 10. 작업 요청 빠른 참조

### 자주 쓰는 요청 패턴

```
"P[번호] [단계]단계 — [구체적 작업]"

예시:
"P1 1단계 — 데이터셋 확보"
"P2 2단계 — dbt 라이브러리 매핑과 SQLD 커버리지 정리"
"P3 3단계 — PostGIS 공간 쿼리 코드 구현"
"P5 4단계 — Deck.gl H3HexagonLayer 시각화 코드"
"P6 면접 대비 — 기술 선택 이유 정리"
"전체 일정 점검 — 현재 진행 상황 리뷰"
```

### 상태 업데이트 요청

```
"P1 완료 — 상태 업데이트해줘"
"이번 주 W3 작업 회고해줘"
```

---

*최종 업데이트: 2026-04-05*  
*다음 작업: P1 1단계 — 데이터셋 확보*

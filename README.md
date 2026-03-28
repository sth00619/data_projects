# 📊 Data & Backend Portfolio Projects

> 데이터 엔지니어 / 데이터 분석가 / 백엔드 개발자 취업을 목표로 설계된 5개 포트폴리오 프로젝트 모음입니다.
> 각 프로젝트는 독립 레포지토리로 관리되며, 이 레포는 **Git Submodule** 구조로 통합 관리합니다.

---

## 🗂️ 프로젝트 목록

| # | 레포 | 주제 | 핵심 기술 |
|---|------|------|-----------|
| 1 | [fraud-detection-dashboard](https://github.com/sth00619/fraud-detection-dashboard) | 실시간 금융 거래 이상탐지 대시보드 | Airflow · XGBoost · FastAPI · Next.js |
| 2 | [customer-churn-platform](https://github.com/sth00619/customer-churn-platform) | SaaS 고객 이탈 예측 & 코호트 분석 | Spring Boot · dbt · LightGBM · D3.js |
| 3 | [seoul-transit-delay](https://github.com/sth00619/seoul-transit-delay) | 서울 대중교통 지연 예측 & 경로 최적화 | PostGIS · LSTM · Mapbox GL JS |
| 4 | [kbeauty-trend-forecast](https://github.com/sth00619/kbeauty-trend-forecast) | K-뷰티 글로벌 트렌드 분석 & 수요 예측 | Prophet · Elasticsearch · Spring Boot |
| 5 | [seoul-store-locator](https://github.com/sth00619/seoul-store-locator) | 서울 상권 분석 & 점포 입지 추천 | H3 · PostGIS · GWR · Deck.gl |

---

## ⚡ 추천 개발 순서

```
P1 (Fraud)    → 파이프라인 + ML + API 기본기
P2 (Churn)    → Spring Boot + dbt + Bayesian A/B
P3 (Transit)  → PostGIS + 공간데이터 + LSTM
P5 (Location) → 가장 복합적인 공간 분석
P4 (K-Beauty) → NLP + Elasticsearch + 다양한 외부 API
```

---

## 🛠️ 공통 인프라 스택

```
Language  : Python 3.11+ / Java 17 / TypeScript
Workflow  : Apache Airflow / Prefect
DB        : PostgreSQL 16 + PostGIS + Redis
ML        : scikit-learn · LightGBM · XGBoost · Prophet · Keras
Backend   : FastAPI / Spring Boot 3.x
Frontend  : Next.js 14 + Tailwind CSS
Infra     : Docker Compose · GitHub Actions
```

---

## 📥 전체 클론 방법

```bash
git clone --recurse-submodules https://github.com/sth00619/data_projects.git
# 이미 클론한 경우
git submodule update --init --recursive
```

---

## 📈 역량 커버리지

| 역량 | P1 | P2 | P3 | P4 | P5 |
|------|----|----|----|----|-----|
| ETL 파이프라인 | ✅ Airflow | ✅ Prefect | ✅ Airflow | ✅ Airflow | ✅ Airflow |
| SQL / DB 설계 | ✅ | ✅ Star | ✅ PostGIS | ✅ | ✅ H3 |
| ML 모델링 | ✅ 이상탐지 | ✅ 이탈예측 | ✅ 시계열 | ✅ Prophet | ✅ GBM+GWR |
| A/B 테스트 | ✅ 빈도주의 | ✅ Bayesian | ✅ | ✅ 모델비교 | ✅ 백테스트 |
| REST API | ✅ FastAPI | ✅ Spring | ✅ FastAPI | ✅ Spring | ✅ FastAPI |
| 데이터 시각화 | ✅ Recharts | ✅ D3.js | ✅ Mapbox | ✅ Choropleth | ✅ Deck.gl |
| Docker / CI/CD | ✅ | ✅ | ✅ | ✅ | ✅ |
| 공간 데이터 | - | - | ✅ PostGIS | - | ✅ H3+GWR |

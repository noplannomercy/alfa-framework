# ALFA (AI/LLM Framework for Adoption)

기업이 LLM을 조직에 도입할 때 거치는 전체 프로세스를 체계화한 프레임워크.

```
ALFA (도입) → IRM (설계) → 구현/운영
```

---

## 왜 ALFA인가

LLM 도입 방법론이 아직 없다. 클라우드 도입(AWS CAF), AI 위험관리(NIST AI RMF), AI 관리체계(ISO 42001)는 있지만, **"LLM을 조직에 도입하는 A to Z"를 단계별로 안내하는 실행 프레임워크**는 존재하지 않는다.

---

## 구조

```
Phase 0: WHY      — 목적 정의 (비즈니스 문제, KPI)
Phase 1: ASSESS   — 조직 준비도 (데이터, 인재, 인프라, 규제)
Phase 2: GOVERN   — 거버넌스 & 정책 (필수/선택 분리)
Phase 3: PLATFORM — 인프라 & 기술 기반
Phase 4: PILOT    — 파일럿 실행 (★ IRM 투입)
Phase 5: SCALE    — 프로덕션 전환 & 확산 (종확산/횡확산)
Phase 6: OPERATE  — 운영 & 지속 개선 (순환)
```

### 원칙

1. **검증 전 과투자 금지** — API로 시작, 데이터로 판단, 필요 시 승격
2. **각 Phase에 Owner 지정** — 소유자 없는 Phase는 실행되지 않는다
3. **People은 Phase가 아니라 모든 Phase에 내장** — BCG: AI 성공의 70%는 사람/프로세스/문화

---

## 문서 목록

### 코어
- [ALFA Framework v1](ALFA_Framework_v1.md) — 프레임워크 본문

### 시뮬레이션 (examples/)

| 업종 | 미팅 | 거버넌스 | 일정 | 특성 |
|------|:---:|---------|------|------|
| [금융 (현대캐피탈)](examples/hyundai-capital/) | 2회 | 무거움 | 3~4개월 | 금감원, 컴플라이언스 별도 |
| [IT서비스](examples/itservice-company/) | 1회 | 가벼움 | 한 달 | 미팅 1회로 Phase 0~3 끝 |
| [제조 (자동차 부품)](examples/manufacturing-company/) | 1+1회 | 가벼움 | 3개월 | 온프레미스, 파일럿 후 확산 |
| [이커머스](examples/ecommerce-company/) | 1회 | 가벼움→무거워질 예정 | 한 달 | 고객 대면 전환 변수 |

### ALFA→IRM 연결 결과 (examples/irm-results/)

| 유즈케이스 | IRM 결과 | 핵심 |
|-----------|---------|------|
| [제조: 불량 원인 분석](examples/irm-results/manufacturing-defect-analysis/) | 탐색 중심, GraphRAG 필수 | 같은 도메인이라도... |
| [제조: 검사 절차 자동화](examples/irm-results/manufacturing-inspection/) | 실행(확정) 중심, GraphRAG 불필요 | ...유즈케이스가 다르면 IRM 결과가 다르다 |
| [이커머스: CS 상담사 보조](examples/irm-results/ecommerce-cs-assistant/) | 탐색+접근만, 가장 단순 | |

---

## ALFA ↔ IRM 관계

ALFA는 "LLM을 조직에 어떻게 들여놓을까", [IRM](https://github.com/noplannomercy/irm-framework)은 "에이전트한테 일을 어떻게 시킬까".

```
ALFA Phase 0~3: 도입 준비
ALFA Phase 4:   유즈케이스 정의서 → ★ IRM 투입 ★
ALFA Phase 5~6: 확산 + 운영 (유즈케이스 추가 시 Phase 4 반복)
```

---

## 시작하기

1. [ALFA Framework v1](ALFA_Framework_v1.md) 읽기
2. [examples/](examples/) 중 자기 업종과 비슷한 케이스 참조
3. 고객 프로필 양식 채우기 (ALFA 코어에 양식 있음)
4. Phase 0~3 수행 → Phase 4에서 IRM 투입

---

## 라이선스

MIT

# 서민혁 | Backend Developer

기획 의도를 데이터 규칙과 API 계약으로 구체화하고,  
예외 상황에서도 그 규칙이 유지되는지 테스트로 검증합니다.

이전에는 기획과 UI/UX 업무를 담당하며 화면 정의서와 협업 문서를 작성했습니다.  
현재는 사용자 흐름과 상태 변화를 데이터 모델, API, 테스트로 연결하는 백엔드 개발에 집중하고 있습니다.

---

## Featured Project

### Rebalance — 장기 투자자를 위한 포트폴리오 리밸런싱 서비스
[Repository](https://github.com/wasw2123/rebalance-backend-public) · [Portfolio](https://app.notion.com/p/Rebalance-3c47084d06cd8051834af078e2fdbadc)

사용자가 목표 비중을 설정하면 현재 포트폴리오와의 차이를 계산하고,  
실행 가능한 매수·매도 수량과 리밸런싱 시점을 안내하는 개인 프로젝트입니다.

**주요 구현**

- 상대 가중치와 절대 비중을 함께 지원하는 리밸런싱 계산 엔진
- 장기 보유 종목을 전체 자산 가치에는 포함하고 매매 계산에서는 제외하는 자산 모델
- 정상 상태에서 임계값 초과 상태로 전환되는 순간에만 알림을 생성하는 상태 머신
- 가격 캐시와 가격 변경 fan-out, 시장별 정기 점검을 결합한 괴리율 평가
- Web·Mobile 환경을 구분한 Refresh Token 전달과 Token Rotation
- 일간 자산 스냅샷, 보유 수량 변화 계산, 투자 메모 관리
- 단위·서비스·PostgreSQL E2E 테스트와 GitHub Actions 기반 CI/CD

**Tech Stack**  
`Python` `FastAPI` `PostgreSQL` `SQLAlchemy Async` `Alembic` `APScheduler` `FCM` `Docker` `AWS`

---

## How I Work

- 화면 요구사항을 데이터의 기준 시점과 상태 전이로 구체화합니다.
- 정상 흐름뿐 아니라 권한, 중복 요청, 외부 API 장애와 복구 기준을 함께 정의합니다.
- 구현 의도를 API 명세와 기술 문서로 공유하고 테스트로 경계 조건을 고정합니다.
- 복잡성을 먼저 추가하기보다 현재 규모에서 필요한 구조를 선택하고 확장 경계를 남깁니다.

---

## Tech Stack

| Area | Technologies |
| --- | --- |
| Backend | Python, FastAPI, Django, Django REST Framework |
| Data | PostgreSQL, pgvector, Redis, SQLAlchemy, Django ORM |
| Async·External | Celery, APScheduler, FCM, AWS S3, REST API Integration |
| Infra·Quality | Docker, Nginx, Caddy, AWS EC2·RDS, GitHub Actions, pytest, mypy, Ruff |

---

## Contact

- GitHub: [@wasw2123](https://github.com/wasw2123)
- Portfolio: [노션](https://app.notion.com/p/3957084d06cd805a8b59d667f965cf37?source=copy_link)
- Email: wasw2123@gmail.com

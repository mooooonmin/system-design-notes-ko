# 번역 가이드

[liquidslr/system-design-notes](https://github.com/liquidslr/system-design-notes)를 한국어로 옮길 때 지키는 원칙과 용어입니다.

## 원칙

- **문체**: 노트이므로 평서체("~한다", "~이다")로 쓴다. 목록 항목은 명사형 종결("~함", "~가능")이나 짧은 구로 끝내도 된다.
- **용어**: 아래 용어집을 따른다. 처음 나올 때만 `한국어(English)` 형태로 원어를 함께 적고, 그 뒤로는 한국어만 쓴다.
  - 한국어로 옮기면 오히려 어색한 용어(API, CDN, 해시, 샤딩, 캐시 등)는 그대로 음차하거나 영어로 둔다.
- **고유명사**: 제품·서비스·회사 이름(Redis, Kafka, Cassandra, Amazon S3 등)과 알고리즘 이름(Snowflake 등)은 영어 그대로 둔다.
- **코드와 수치**: 코드 블록, 명령어, SQL, API 경로, 수식, 숫자는 바꾸지 않는다.
- **이미지**: 다이어그램은 원본 그대로 쓴다. `alt` 텍스트만 한국어로 옮긴다.
- **구조**: 제목 수준, 목록, 표, `<div>`/`<img>` 같은 HTML 구조와 이미지 경로는 원본과 똑같이 유지한다.
- **폴더명**: 원본 폴더명을 그대로 써서 링크와 원본 업데이트 병합이 깨지지 않게 한다.
- **원문 오류**: 원문에 명백한 오타가 있으면 바로잡아 옮기고, 내용상 의문이 있으면 원문 의미를 그대로 살린다.

## 용어집

| 영어 | 한국어 |
|---|---|
| scale / scalability | 규모 확장 / 규모 확장성 |
| vertical scaling (scale up) | 수직적 규모 확장(스케일 업) |
| horizontal scaling (scale out) | 수평적 규모 확장(스케일 아웃) |
| load balancer | 로드밸런서 |
| replication | 다중화(데이터베이스) / 복제(데이터) |
| failover | 장애 조치(failover) |
| cache / cache tier | 캐시 / 캐시 계층 |
| eviction policy | 캐시 방출 정책 |
| stateless / stateful | 무상태 / 상태 유지 |
| data center | 데이터 센터 |
| message queue | 메시지 큐 |
| producer / consumer | 생산자 / 소비자 |
| sharding / shard key | 샤딩 / 샤드 키 |
| hotspot / celebrity problem | 핫스팟 / 유명인 문제 |
| back-of-the-envelope estimation | 개략적인 규모 추정 |
| QPS (queries per second) | 초당 질의 수(QPS) |
| latency / throughput | 지연 시간 / 처리량 |
| availability | 가용성 |
| rate limiter / throttle | 처리율 제한 장치 / 처리율 제한(스로틀링) |
| token bucket / leaking bucket | 토큰 버킷 / 누출 버킷 |
| fixed window counter / sliding window log | 고정 윈도 카운터 / 이동 윈도 로그 |
| consistent hashing / hash ring | 안정 해시 / 해시 링 |
| virtual node | 가상 노드 |
| key-value store | 키-값 저장소 |
| consistency / eventual consistency | 일관성 / 결과적 일관성 |
| partition / partition tolerance | 파티션 / 파티션 감내 |
| quorum consensus | 정족수 합의 |
| vector clock | 벡터 시계 |
| gossip protocol | 가십 프로토콜 |
| sloppy quorum / hinted handoff | 느슨한 정족수 / 단서 후 임시 위탁 |
| Merkle tree | 머클 트리 |
| unique ID generator | 유일 ID 생성기 |
| URL shortener | URL 단축기 |
| redirect | 리디렉션 |
| web crawler | 웹 크롤러 |
| URL frontier | 미수집 URL 저장소(URL frontier) |
| politeness / prioritizer | 예의 / 우선순위 결정 장치 |
| notification | 알림 |
| news feed / fanout on write / fanout on read | 뉴스 피드 / 쓰기 시점 팬아웃 / 읽기 시점 팬아웃 |
| long polling / WebSocket | 롱 폴링 / 웹소켓 |
| presence | 접속 상태 |
| heartbeat | 박동(heartbeat) |
| autocomplete / trie | 자동완성 / 트라이 |
| transcoding / DAG | 트랜스코딩 / DAG(방향성 비순환 그래프) |
| pre-signed URL | 사전 서명된 URL |
| block server / delta sync | 블록 저장소 서버 / 델타 동기화 |
| proximity service / geohash / quadtree | 근접성 서비스 / 지오해시 / 쿼드트리 |
| geospatial index | 지리 공간 색인 |
| map tile / routing tile | 지도 타일 / 경로 안내 타일 |
| ETA | 도착 예정 시간(ETA) |
| pub/sub | 발행/구독(pub/sub) |
| topic / partition / broker | 토픽 / 파티션 / 브로커 |
| consumer group / rebalancing | 소비자 그룹 / 재조정 |
| in-sync replicas (ISR) | 동기화된 사본(ISR) |
| at-most-once / at-least-once / exactly-once | 최대 한 번 / 최소 한 번 / 정확히 한 번 |
| write-ahead log (WAL) | 선행 기록 로그(WAL) |
| metrics / alerting | 지표 / 경보 |
| time-series database | 시계열 데이터베이스 |
| pull model / push model | 풀 모델 / 푸시 모델 |
| aggregation / watermark | 집계 / 워터마크 |
| tumbling window / sliding window | 텀블링 윈도 / 슬라이딩 윈도 |
| reconciliation | 대사(reconciliation) |
| idempotency | 멱등성 |
| optimistic / pessimistic locking | 낙관적 / 비관적 잠금 |
| double booking | 이중 예약 |
| object storage / bucket | 객체 저장소 / 버킷 |
| erasure coding | 소거 코드(erasure coding) |
| leaderboard / sorted set | 순위표 / 정렬 집합 |
| payment service provider (PSP) | 결제 대행사(PSP) |
| double-entry ledger | 복식부기 원장 |
| distributed transaction / 2PC / TC/C / Saga | 분산 트랜잭션 / 2단계 커밋 / TC/C / 사가 |
| event sourcing / CQRS | 이벤트 소싱 / CQRS |
| state machine | 상태 기계 |
| order book / matching engine / sequencer | 호가 창 / 체결 엔진 / 시퀀서 |

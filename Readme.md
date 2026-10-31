# [System Design Interview - An Insider's Guide (Vol 1 and 2)](https://bytebytego.com/courses/system-design-interview) 한국어 노트

> **번역본 안내**
> 이 저장소는 [liquidslr/system-design-notes](https://github.com/liquidslr/system-design-notes)를 한국어로 옮긴 **비공식 번역본**입니다.
> 원본 노트의 저작권은 원작자에게 있으며, 노트의 바탕이 된 책의 저작권은 저자 Alex Xu(및 Sahn Lam)와 출판사에 있습니다.
> 다이어그램 이미지는 원본 그대로이므로 그림 속 글자는 영어입니다.
> 번역 원칙과 용어는 [TRANSLATION.md](./TRANSLATION.md)를 참고하세요.

이 노트는 『System Design Interview』 [1권과 2권(2판)](https://www.goodreads.com/book/show/54109255-system-design-interview-an-insider-s-guide)을 바탕으로 정리한 것입니다.
국내에는 『가상 면접 사례로 배우는 대규모 시스템 설계 기초』 1·2권으로 번역 출간되어 있습니다.

원본 노트 웹 버전: https://pagefy.io/system-design/system-design-interview-by-alex-xu

**참고:** 원본 노트는 아직 작성 중입니다.

### 1권

 * [1장 - 사용자 수에 따른 규모 확장성](./01.%20Scaling/)
 * [2장 - 개략적인 규모 추정](./02.%20Back%20Of%20the%20Envelope%20Estimation/)
 * [3장 - 시스템 설계 면접 공략법](./03.%20System%20Design%20Framework/)
 * [4장 - 처리율 제한 장치 설계](./04.%20Rate%20Limiter/)
 * [5장 - 안정 해시 설계](./05.%20Consistent%20Hashing/)
 * [6장 - 키-값 저장소 설계](./06.%20Key-Value%20Store/)
 * [7장 - 분산 시스템을 위한 유일 ID 생성기 설계](./07.%20Unique-Id%20Generator/)
 * [8장 - URL 단축기 설계](./08.%20URL%20Shortener/)
 * [9장 - 웹 크롤러 설계](./09.%20Web%20Crawler/)
 * [10장 - 알림 시스템 설계](./10.%20Notification%20System/)
 * [11장 - 뉴스 피드 시스템 설계](./11.%20News%20Feed%20System/)
 * [12장 - 채팅 시스템 설계](./12.%20Chat%20System/)
 * [13장 - 검색어 자동완성 시스템 설계](./13.%20Search%20Autocomplete/)
 * [14장 - 유튜브 설계](./14.%20Youtube/)
 * [15장 - 구글 드라이브 설계](./15.%20Google%20Drive/)

### 2권

 * [16장 - 근접성 서비스](./16.%20Proximity%20Service/)
 * [17장 - 주변 친구](./17.%20Nearby%20Friends/)
 * [18장 - 구글 맵 설계](./18.%20Google%20Maps/)
 * [19장 - 분산 메시지 큐](./19.%20Distributed%20Message%20Queue/)
 * [20장 - 지표 모니터링 및 경보 시스템](./20.%20Metrics%20Monitoring%20and%20Alerting%20System/)
 * [21장 - 광고 클릭 이벤트 집계](./21.%20Ad%20Click%20Event%20Aggregation/)
 * [22장 - 호텔 예약 시스템](./22.%20Hotel%20Reservation%20System/)
 * [23장 - 분산 이메일 서비스](./23.%20Distributed%20Email%20Service/)
 * [24장 - S3와 유사한 객체 저장소](./24.%20S3-like%20Object%20Storage/)
 * [25장 - 실시간 게임 순위표](./25.%20Real-time%20Gaming%20Leaderboard/)
 * [26장 - 결제 시스템](./26.%20Payment%20System/)
 * [27장 - 전자 지갑](./27.%20%20Digital%20Wallet/)
 * [28장 - 증권 거래소](./28.%20Stock%20Exchange/)


# 추가 자료

링크된 자료는 대부분 영어 문서이므로 제목을 원문 그대로 두었습니다.

### 처리율 제한
- [Circuit Breaker Algorithm](https://martinfowler.com/bliki/CircuitBreaker.html)
- [Uber Rate Limiter](https://github.com/uber-go/ratelimit/blob/master/ratelimit.go)


### 안정 해시
- [Consistent Hashing](https://tom-e-white.com/2007/11/consistent-hashing.html)
- [CS168: Introduction and Consistent Hashing:]( http://theory.stanford.edu/~tim/s16/l/l1.pdf)
- [Apache Cassandra](http://www.cs.cornell.edu/Projects/ladis2009/papers/Lakshman-ladis2009.PDF)
- [Scaling Discord](https://blog.discord.com/scaling-elixir-f9b8e1e7c29b)
- [Google Maglev](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44824.pdf)


### 키-값 저장소
- [Amazon Dynamo](https://www.allthingsdistributed.com/files/amazon-dynamo-sosp2007.pdf)
- [Cassandra Architecture](https://docs.datastax.com/en/archived/cassandra/3.0/cassandra/architecture/archIntro.html)
- [Google BigTable Architecture](https://static.googleusercontent.com/media/research.google.com/en//archive/bigtable-osdi06.pdf)
- [Amazon Dynamo DB Internals](https://www.allthingsdistributed.com/2007/10/amazons_dynamo.html)
- [Design Patterns in Amazon Dynamo DB](https://www.youtube.com/watch?v=HaEPXoXVf2k)
- [Internals of Amazon Dynamo DB](https://www.youtube.com/watch?v=yvBR71D0nAQ)


### 유일 ID 생성기
- [Ticket Servers: Distributed Unique Primary Keys on the Cheap](https://code.flickr.net/2010/02/08/ticket-servers-distributed-unique-primary-keys-on-the-cheap)
- [Snowflake](https://blog.twitter.com/engineering/en_us/a/2010/announcing-snowflake.html)


### 웹 크롤러
- [Web Crawling](http://infolab.stanford.edu/~olston/publications/crawling_survey.pdf)
- [Google Dynamic Rendering](https://developers.google.com/search/docs/guides/dynamic-rendering)



### 채팅 시스템
- [How Discord stores billions of messages](https://discord.com/blog/how-discord-stores-billions-of-messages)
- [Flannel: An Application-Level Edge Cache to Make Slack Scale](https://slack.engineering/flannel-an-application-level-edge-cache-to-make-slack-scale/)


### 검색어 자동완성
- [How We Built Prefixy](https://medium.com/@prefixyteam/how-we-built-prefixy-a-scalable-prefix-search-service-for-powering-autocomplete-c20f98e2eff1)
- [Prefix Hash Tree](https://people.eecs.berkeley.edu/~sylvia/papers/pht.pdf)


### 유튜브
- [YouTube Architecture](http://highscalability.com/youtube-architecture)
- [YouTube scalability 2012](https://www.youtube.com/watch?v=w5WVu624fY8)
- [Transcoding Videos at Scale](https://www.egnyte.com/blog/2018/12/transcoding-how-we-serve-videos-at-scale/)
- [Facebook Video Broadcasting](https://engineering.fb.com/ios/under-the-hood-broadcasting-live-video-to-millions/)
- [Netflix Video Encoding at Scale](https://netflixtechblog.com/high-quality-video-encoding-at-scale-d159db052746)
- [Netflix Shot based encoding](https://netflixtechblog.com/optimized-shot-based-encodes-now-streaming-4b9464204830)


### 구글 드라이브
- [Differential Synchronization](https://neil.fraser.name/writing/sync/)
- [Differential Synchronization Video](https://www.youtube.com/watch?v=S2Hp_1jqpY8)
- [How We’ve Scaled Dropbox](https://www.youtube.com/watch?v=PE4gwstWhmc&feature=youtu.be)

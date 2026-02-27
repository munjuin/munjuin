# 안녕하세요, 코드의 '작동'보다 작동하는 '원리'에 집중하는 백엔드 개발자 문주인입니다.

"단순 기능 구현"보다 **"기술적 한계를 어떻게 극복했는가"**와 **"왜 이 기술을 선택했는가(First Principles)"**를 집요하게 봅니다. 바퀴를 다시 발명하며 원리를 이해하는 과정을 즐기며, 최근에는 보안 중심의 로컬 LLM과 RAG 파이프라인 연동을 통한 지능형 업무 자동화 시스템 구축에 집중하고 있습니다.

---

##  Tech Stack

| Classification | Technology |
| --- | --- |
| **Language** | TypeScript, JavaScript |
| **Backend** | Node.js, Express, NestJS |
| **Database** | PostgreSQL (`pgvector`), MySQL, Redis |
| **DevOps & AI** | Docker, LangChain, Ollama (Llama 3), GitHub Actions, NPM |

---

##  Projects Highlight

*아래 Pinned Repositories 프로젝트들의 **개발 의도(Why & How)***입니다.

### 1. Local AI Office Automator (사내 문서 특화 RAG AI 비서)
> **"보안이 중요한 사내 문서를 외부 유출 없이 처리하는 로컬 LLM 시스템 구축"**
* **문제 의식:** 민감한 사내 문서를 외부 클라우드 AI(ChatGPT 등)에 전송할 때 발생하는 데이터 보안 위험을 원천 차단하고자 했습니다.
* **해결 접근:**
  * LangChain과 Ollama(Llama 3)를 활용하여 100% 로컬 환경에서 동작하는 **RAG(검색 증강 생성) 파이프라인**을 설계했습니다.
  * PostgreSQL의 `pgvector` 기반 코사인 유사도 벡터 검색 엔진을 구축하고, `RecursiveCharacterTextSplitter`를 활용한 텍스트 청킹으로 검색 품질을 최적화했습니다.
  * API 응답 속도 향상과 HTTP의 Stateless 한계 극복을 위해 **Redis**를 도입, 대화 세션 유지 및 캐싱 레이어를 적용했습니다.
  * 이진 파일(PDF) 파싱 중 발생하는 Null Byte(`\x00`) 데이터 오염을 정규식으로 방어하여 DB 무결성을 확보하는 데이터 정제 레이어를 추가했습니다.

### 2. create-express-esm (NPM 오픈소스 / CLI 도구)
> **"내가 불편해서 직접 만든 개발자 경험(DX) 개선 도구"**
* **문제 의식:** 기존 Express 생성기가 CJS 기반이라, 최신 ESM 문법을 적용하려면 매번 초기 설정에 시간을 낭비해야 했습니다.
* **해결 접근:** `npm init` 한 번으로 최신 스택(ESM)이 적용된 보일러플레이트를 자동 생성하는 CLI 도구를 직접 개발하여 NPM에 배포(v1.2.2)했습니다.

### 3. ts-lodashtype-definition
> **"타입 시스템의 한계를 시험하고 정교한 설계 능력 기르기"**
* **문제 의식:** 유틸리티 라이브러리가 어떻게 완벽한 타입 추론을 제공하는지 그 원리가 궁금했습니다.
* **해결 접근:** Lodash 핵심 함수들에 Generics, Conditional Types, Mapped Types를 적용하여 직접 타입을 재구현하며 TypeScript의 정적 분석 원리를 탐구했습니다.

### 4. Jewelry Shop Project (이커머스)
> **"라이브러리 없이 순수 아키텍처 원리 구축하기"**
* **문제 의식:** 프레임워크의 자동화 이면에 있는 MVC 패턴과 DB 설계의 중요성을 체감하고 싶었습니다.
* **해결 접근:** RDBMS 기반 ERD 설계와 트랜잭션 관리를 통해 데이터 일관성을 확보하고, Express에서 NestJS로 마이그레이션하며 확장성 있는 서버를 구축하고 있습니다.

---

##  Migration & Learning Roadmap

현재 완성된 MVP들을 바탕으로 기술적 성장을 위한 단계적 고도화를 진행하고 있습니다.

1. **Step 1.** Pure JS / Express 기반 핵심 MVP 기능 완성
2. **Step 2.** TypeScript 마이그레이션: 정적 타입을 도입하여 코드 품질 및 유지보수성 향상
3. **Step 3.** NestJS 전환: 의존성 주입(DI)과 모듈화 구조를 도입하여 확장 가능한 백엔드 구축
4. **Step 4.** Advanced Architecture: Redis 인메모리 캐싱 및 AI(RAG) 파이프라인 융합 (현재 진행 중)

---

##  Contact

언제든 소통을 환영합니다.
* **Email:** raiawa1212@gmail.com
* **GitHub:** [https://github.com/munjuin](https://github.com/munjuin)

# 안녕하세요, 코드의 '작동'보다 작동하는 '원리'에 집중하는 백엔드 개발자 문주인입니다.

> **"단순 기능 구현"보다 "기술적 한계를 어떻게 극복했는가"와 "왜 이 기술을 선택했는가"를 집요하게 봅니다.**
> 바퀴를 다시 발명하며 원리를 이해하는 과정을 즐기며, 현재는 구축한 MVP 서비스를 견고한 아키텍처로 마이그레이션하며 시스템의 안정성을 고민하고 있습니다.

<br>

## 🛠 Tech Stack
**Fundamental & Backend & AI Ops**

| Classification | Technology |
| :--- | :--- |
| **Language** | ![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=TypeScript&logoColor=white) ![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=JavaScript&logoColor=black) ![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=Node.js&logoColor=white) |
| **Framework** | ![NestJS](https://img.shields.io/badge/-NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white) ![Next.js](https://img.shields.io/badge/-Next.js-000000?style=flat-square&logo=next.js&logoColor=white) ![Express](https://img.shields.io/badge/-Express-000000?style=flat-square&logo=Express&logoColor=white) |
| **Database** | ![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=PostgreSQL&logoColor=white) ![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white) |
| **Tools & AI** | ![LangChain](https://img.shields.io/badge/-LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![Ollama](https://img.shields.io/badge/-Ollama-000000?style=flat-square&logo=ollama&logoColor=white) ![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=Docker&logoColor=white) ![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white) |

<br>

## 🚀 Projects Highlight
*아래 Pinned Repositories 프로젝트들의 **개발 의도(Why & How)**입니다.*

### 1. Local AI Office Automator (v1.0.0 Completed)
**"NestJS & Next.js 기반의 100% On-Premise RAG 솔루션"**
- **문제 의식:** 민감한 사내 문서를 외부 클라우드(GPT 등)에 전송하지 않고, 로컬 환경에서 안전하게 분석하고 대화할 수 있는 시스템이 필요했습니다.
- **해결 접근:** - **Full-Stack RAG:** `NestJS`(백엔드)와 `Next.js`(프론트엔드)를 통합하고 `pgvector`를 활용해 벡터 검색 파이프라인을 직접 구축했습니다.
    - **Engineering Depth:** 긴 문서 처리를 위한 **Recursive Chunking(1000자)** 알고리즘과 멀티 턴 대화를 위한 **Session Memory** 아키텍처를 설계하여 LLM의 한계(Context Window, Hallucination)를 극복했습니다.

### 2. create-express-esm (NPM Package)
**"반복되는 초기 설정의 자동화와 최신 표준(ESM) 도입"**
- **문제 의식:** 기존 도구들이 CJS 기반인 점에 불편함을 느껴, ESM 환경을 즉시 구축할 수 있는 CLI 도구를 개발했습니다.
- **해결 접근:** `npm init` 명령어로 즉시 실행 가능한 보일러플레이트 생성기를 배포하여 개발 생산성을 개선했습니다.

### 3. Jewelry Shop Project
**"프레임워크 없이 순수 Node.js로 구축하는 견고한 아키텍처"**
- **문제 의식:** 추상화된 프레임워크 뒤에 숨겨진 `MVC 패턴`과 `DB 설계`의 본질을 직접 체감하고 싶었습니다.
- **해결 접근:** 현재 JS 기반의 MVP를 **TypeScript로 마이그레이션** 중이며, JSON 타입을 활용한 유연한 옵션 설계로 대규모 데이터 처리의 안정성을 확보하고 있습니다.

### 4. ts-lodashtype-definition
**"타입 시스템의 한계를 시험하고 정교한 설계 능력 기르기"**
- **문제 의식:** 복잡한 유틸리티 라이브러리가 어떻게 전 세계 개발자에게 완벽한 추론을 제공하는지 그 원리가 궁금했습니다.
- **해결 접근:** `Generics`, `Conditional Types`, `Mapped Types`를 활용해 Lodash 핵심 함수를 직접 정의하며 **정적 분석의 신뢰성**을 극대화했습니다.

<br>

## 🗺️ Migration & Growth Roadmap
**단순 구현을 넘어 기술적 고도화를 위한 단계적 여정입니다.**

- [x] **Step 1. Fundamental Focus**: Pure JS / Express 기반 핵심 기능 및 CLI 도구 완성
- [x] **Step 2. Type Safety**: 핵심 프로젝트의 **TypeScript 마이그레이션** 및 타입 안정성 확보
- [x] **Step 3. Architecture Scaling**: **NestJS 모듈형 아키텍처 도입** 및 RAG 시스템 구축 완료 (`Local AI Automator`)
- [x] **Step 4. Full-stack Integration**: **Next.js 기반 웹 인터페이스** 연동 및 사용자 경험(UX) 고도화
- [ ] **Step 5. Performance & Ops**: Redis 캐싱 도입을 통한 응답 속도 개선 및 Docker Compose 최적화

<br>

## 📬 Contact
**언제든 기술적인 토론과 소통을 환영합니다.**

| Channel | Address |
| :--- | :--- |
| <a href="mailto:raiawa1212@gmail.com"><img src="https://img.shields.io/badge/Gmail-d14836?style=flat-square&logo=Gmail&logoColor=white"/></a> | **raiawa1212@gmail.com** |
| <a href="https://github.com/munjuin"><img src="https://img.shields.io/badge/GitHub-100000?style=flat-square&logo=github&logoColor=white"/></a> | **https://github.com/munjuin** |

# .github


<!--
================================================================================
  오픈소스 README 종합 템플릿
  - 필요한 섹션만 발췌해서 사용하세요.
  - `<!-- -->` 주석은 작성 가이드입니다. 완성 후 삭제하세요.
  - {{ }} 로 감싼 부분은 실제 값으로 치환하세요.
================================================================================
-->

<!-- ========== 1. 헤더 영역 ========== -->

<div align="center">

<!-- 로고 / 배너 이미지 -->
<img src="docs/assets/logo.png" alt="{{PROJECT_NAME}} logo" width="180" />

# {{PROJECT_NAME}}

**{{한 줄 소개 — 이게 뭐고 왜 쓰는지 한 문장으로}}**

<!-- 배지(badges): shields.io 에서 생성 -->
[![Build Status](https://img.shields.io/github/actions/workflow/status/{{OWNER}}/{{REPO}}/ci.yml?branch=main)](https://github.com/{{OWNER}}/{{REPO}}/actions)
[![Coverage](https://img.shields.io/codecov/c/github/{{OWNER}}/{{REPO}})](https://codecov.io/gh/{{OWNER}}/{{REPO}})
[![npm version](https://img.shields.io/npm/v/{{PACKAGE_NAME}})](https://www.npmjs.com/package/{{PACKAGE_NAME}})
[![Downloads](https://img.shields.io/npm/dm/{{PACKAGE_NAME}})](https://www.npmjs.com/package/{{PACKAGE_NAME}})
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

[문서](https://{{DOCS_URL}}) · [데모](https://{{DEMO_URL}}) · [버그 신고](https://github.com/{{OWNER}}/{{REPO}}/issues) · [기능 제안](https://github.com/{{OWNER}}/{{REPO}}/discussions)

<!-- 다국어 README -->
[English](README.md) · [한국어](README.ko.md) · [日本語](README.ja.md)

</div>

---

<!-- ========== 목차 ========== -->
## 목차

- [소개](#소개)
  - [주요 기능](#주요-기능)
  - [데모](#데모)
  - [왜 이 프로젝트인가](#왜-이-프로젝트인가)
- [시작하기](#시작하기)
  - [요구사항](#요구사항)
  - [설치](#설치)
  - [빠른 시작](#빠른-시작)
  - [기본 사용법](#기본-사용법)
- [상세 문서](#상세-문서)
  - [설정](#설정)
  - [API 레퍼런스](#api-레퍼런스)
  - [사용 예제](#사용-예제)
  - [아키텍처](#아키텍처)
  - [성능 벤치마크](#성능-벤치마크)
- [개발 및 기여](#개발-및-기여)
  - [개발 환경 설정](#개발-환경-설정)
  - [프로젝트 구조](#프로젝트-구조)
  - [테스트](#테스트)
  - [기여 가이드](#기여-가이드)
  - [커밋 컨벤션](#커밋-컨벤션)
  - [행동 강령](#행동-강령)
- [프로젝트 정보](#프로젝트-정보)
  - [로드맵](#로드맵)
  - [변경 이력](#변경-이력)
  - [알려진 이슈 및 제한사항](#알려진-이슈-및-제한사항)
  - [FAQ](#faq)
  - [트러블슈팅](#트러블슈팅)
  - [라이선스](#라이선스)
- [마무리](#마무리)
  - [기여자](#기여자)
  - [감사의 말](#감사의-말)
  - [후원](#후원)
  - [관련 프로젝트](#관련-프로젝트)
  - [커뮤니티 및 연락처](#커뮤니티-및-연락처)
  - [보안 취약점 신고](#보안-취약점-신고)

---

<!-- ========== 2. 소개 ========== -->
## 소개

{{2~4문장으로 프로젝트가 어떤 문제를 해결하는지 설명합니다.
누가(대상 사용자), 무엇을(핵심 기능), 왜(기존 방식의 문제점) 순서로 쓰면 자연스럽습니다.}}

### 주요 기능

- 🚀 **{{기능 1}}** — {{한 줄 설명}}
- 🔒 **{{기능 2}}** — {{한 줄 설명}}
- 🧩 **{{기능 3}}** — {{한 줄 설명}}
- ⚡ **{{기능 4}}** — {{한 줄 설명}}
- 🌐 **{{기능 5}}** — {{한 줄 설명}}

### 데모

<!-- 스크린샷, GIF, 또는 라이브 데모 링크. 시각적 결과물이 있는 프로젝트라면 사실상 필수입니다. -->

![Demo](docs/assets/demo.gif)

> 라이브 데모: https://{{DEMO_URL}}
> 플레이그라운드: https://{{PLAYGROUND_URL}}

### 왜 이 프로젝트인가

<!-- 유사 프로젝트와의 비교표. 객관적이고 공정하게 작성하세요. -->

| | **{{PROJECT_NAME}}** | {{대안 A}} | {{대안 B}} |
|---|:---:|:---:|:---:|
| {{비교 항목 1}} | ✅ | ❌ | ✅ |
| {{비교 항목 2}} | ✅ | ✅ | ❌ |
| 번들 크기 | {{n}} kB | {{n}} kB | {{n}} kB |
| 의존성 | 0 | {{n}} | {{n}} |
| 라이선스 | MIT | {{...}} | {{...}} |

---

<!-- ========== 3. 시작하기 ========== -->
## 시작하기

### 요구사항

- {{런타임}} {{버전}} 이상 (예: Node.js 18+)
- {{패키지 매니저}} (예: npm 9+ / pnpm 8+)
- {{선택적 의존성}} (예: Docker 24+, PostgreSQL 14+)
- 지원 OS: macOS, Linux, Windows (WSL2 권장)

### 설치

```bash
# npm
npm install {{PACKAGE_NAME}}

# yarn
yarn add {{PACKAGE_NAME}}

# pnpm
pnpm add {{PACKAGE_NAME}}
```

<details>
<summary>다른 설치 방법</summary>

```bash
# Homebrew
brew install {{PACKAGE_NAME}}

# Docker
docker pull {{OWNER}}/{{REPO}}:latest

# 소스에서 빌드
git clone https://github.com/{{OWNER}}/{{REPO}}.git
cd {{REPO}}
make install
```

</details>

### 빠른 시작

<!-- 5분 안에 결과를 볼 수 있는 최소 예제. 복사-붙여넣기만으로 동작해야 합니다. -->

```js
import { createClient } from '{{PACKAGE_NAME}}';

const client = createClient({ apiKey: process.env.API_KEY });

const result = await client.run('hello world');
console.log(result);
//=> { status: 'ok', data: [...] }
```

### 기본 사용법

```js
// 1) 초기화
const client = createClient({
  apiKey: process.env.API_KEY,
  timeout: 5000,
});

// 2) 실행
const result = await client.run(input, { retries: 3 });

// 3) 정리
await client.close();
```

CLI로 사용하는 경우:

```bash
{{CLI_NAME}} run ./input.json --output ./result.json --verbose
```

---

<!-- ========== 4. 상세 문서 ========== -->
## 상세 문서

### 설정

#### 설정 옵션

| 옵션 | 타입 | 기본값 | 설명 |
|---|---|---|---|
| `apiKey` | `string` | — | **(필수)** 인증 키 |
| `timeout` | `number` | `5000` | 요청 타임아웃 (ms) |
| `retries` | `number` | `3` | 실패 시 재시도 횟수 |
| `logLevel` | `'debug' \| 'info' \| 'error'` | `'info'` | 로그 레벨 |

#### 환경 변수

| 변수 | 필수 | 설명 |
|---|:---:|---|
| `API_KEY` | ✅ | 인증 키 |
| `BASE_URL` | ❌ | 기본 엔드포인트 (기본값: `https://api.example.com`) |
| `LOG_LEVEL` | ❌ | 로그 레벨 |

#### 설정 파일

```yaml
# {{project}}.config.yaml
apiKey: ${API_KEY}
timeout: 5000
plugins:
  - name: cache
    options:
      ttl: 3600
```

### API 레퍼런스

<!-- 분량이 많아지면 docs/api.md 로 분리하고 링크만 남기세요. -->

전체 레퍼런스: [docs/api.md](docs/api.md)

#### `createClient(options)`

클라이언트 인스턴스를 생성합니다.

- **파라미터**
  - `options.apiKey` `{string}` — 인증 키
  - `options.timeout` `{number}` — 타임아웃 (ms)
- **반환값** `{Client}`
- **예외** `ConfigError` — 필수 옵션 누락 시

#### `client.run(input, options?)`

- **파라미터**
  - `input` `{string | Buffer}` — 처리할 입력
  - `options.retries` `{number}` — 재시도 횟수
- **반환값** `{Promise<Result>}`

#### CLI 명령어

| 명령어 | 설명 |
|---|---|
| `{{CLI_NAME}} init` | 설정 파일 생성 |
| `{{CLI_NAME}} run <file>` | 실행 |
| `{{CLI_NAME}} validate` | 설정 검증 |

### 사용 예제

더 많은 예제는 [`examples/`](examples/) 디렉터리를 참고하세요.

- [기본 사용](examples/basic) — 최소 구성
- [{{프레임워크}} 연동](examples/with-framework)
- [고급 설정](examples/advanced) — 커스텀 플러그인, 미들웨어
- [프로덕션 배포](examples/production)

### 아키텍처

```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│   Client    │────▶│    Core     │────▶│  Adapter    │
│  (public)   │     │  (pipeline) │     │  (I/O)      │
└─────────────┘     └─────────────┘     └─────────────┘
                           │
                    ┌──────▼──────┐
                    │   Plugins   │
                    └─────────────┘
```

{{각 계층의 역할, 데이터 흐름, 핵심 설계 결정을 2~3문단으로 설명합니다.
"왜 이렇게 만들었는가"를 담으면 기여자에게 큰 도움이 됩니다.}}

자세한 설계 문서: [docs/architecture.md](docs/architecture.md)

### 성능 벤치마크

<!-- 측정 환경을 반드시 명시하세요. 재현 가능해야 신뢰를 얻습니다. -->

측정 환경: {{CPU}}, {{RAM}}, {{OS}}, {{런타임 버전}}

| 시나리오 | {{PROJECT_NAME}} | {{대안 A}} | {{대안 B}} |
|---|---:|---:|---:|
| 콜드 스타트 | {{n}} ms | {{n}} ms | {{n}} ms |
| 처리량 (ops/s) | {{n}} | {{n}} | {{n}} |
| 메모리 사용량 | {{n}} MB | {{n}} MB | {{n}} MB |

재현 방법:

```bash
npm run bench
```

---

<!-- ========== 5. 개발 및 기여 ========== -->
## 개발 및 기여

### 개발 환경 설정

```bash
# 1) 저장소 클론
git clone https://github.com/{{OWNER}}/{{REPO}}.git
cd {{REPO}}

# 2) 의존성 설치
npm install

# 3) 환경 변수 설정
cp .env.example .env

# 4) 개발 서버 실행
npm run dev
```

### 프로젝트 구조

```
{{REPO}}/
├── src/                # 소스 코드
│   ├── core/           # 핵심 로직
│   ├── adapters/       # 외부 연동
│   ├── plugins/        # 플러그인
│   └── index.ts        # 진입점
├── tests/              # 테스트
│   ├── unit/
│   └── integration/
├── examples/           # 사용 예제
├── docs/               # 문서
├── scripts/            # 빌드/유틸 스크립트
└── .github/
    ├── workflows/      # CI/CD
    └── ISSUE_TEMPLATE/
```

### 테스트

```bash
npm test                 # 전체 테스트
npm run test:unit        # 단위 테스트
npm run test:e2e         # E2E 테스트
npm run test:watch       # 워치 모드
npm run test:coverage    # 커버리지 리포트

npm run lint             # 린트
npm run format           # 포맷팅
npm run typecheck        # 타입 검사
```

### 기여 가이드

기여는 언제나 환영합니다! 자세한 내용은 [CONTRIBUTING.md](CONTRIBUTING.md)를 참고하세요.

1. 저장소를 Fork 합니다.
2. 기능 브랜치를 만듭니다. (`git checkout -b feat/amazing-feature`)
3. 변경 사항을 커밋합니다. (`git commit -m 'feat: add amazing feature'`)
4. 브랜치에 Push 합니다. (`git push origin feat/amazing-feature`)
5. Pull Request를 엽니다.

처음 기여하신다면 [`good first issue`](https://github.com/{{OWNER}}/{{REPO}}/labels/good%20first%20issue) 라벨이 붙은 이슈부터 살펴보세요.

### 커밋 컨벤션

[Conventional Commits](https://www.conventionalcommits.org/) 를 따릅니다.

```
<type>(<scope>): <subject>

feat:     새로운 기능
fix:      버그 수정
docs:     문서 변경
style:    코드 포맷팅 (동작 변경 없음)
refactor: 리팩터링
perf:     성능 개선
test:     테스트 추가/수정
chore:    빌드, 설정 등 기타 변경
```

### 행동 강령

모든 참여자는 [행동 강령](CODE_OF_CONDUCT.md)을 준수해야 합니다.

---

<!-- ========== 6. 프로젝트 정보 ========== -->
## 프로젝트 정보

### 로드맵

- [x] {{완료된 항목}}
- [x] {{완료된 항목}}
- [ ] {{v1.1 예정 항목}}
- [ ] {{v2.0 예정 항목}}
- [ ] {{검토 중인 항목}}

전체 로드맵과 논의는 [Discussions](https://github.com/{{OWNER}}/{{REPO}}/discussions)에서 확인하세요.

### 변경 이력

모든 변경 사항은 [CHANGELOG.md](CHANGELOG.md)에 기록됩니다.
버전은 [Semantic Versioning](https://semver.org/lang/ko/)을 따릅니다.

### 알려진 이슈 및 제한사항

- {{제한사항 1}} — {{우회 방법 또는 관련 이슈 링크}}
- {{제한사항 2}}
- {{지원하지 않는 환경/시나리오}}

최신 목록: [Issues](https://github.com/{{OWNER}}/{{REPO}}/issues)

### FAQ

<details>
<summary><b>Q. {{자주 묻는 질문 1}}</b></summary>

{{답변}}

</details>

<details>
<summary><b>Q. {{자주 묻는 질문 2}}</b></summary>

{{답변}}

</details>

<details>
<summary><b>Q. {{대안 A}} 대신 이걸 써야 하나요?</b></summary>

{{솔직하고 균형 잡힌 답변. 어떤 경우엔 다른 도구가 낫다고 말하는 편이 신뢰를 얻습니다.}}

</details>

### 트러블슈팅

<details>
<summary><b>{{에러 메시지 1}}</b></summary>

**원인:** {{원인 설명}}

**해결:**
```bash
{{해결 명령어}}
```

</details>

<details>
<summary><b>{{에러 메시지 2}}</b></summary>

**원인:** {{원인 설명}}
**해결:** {{해결 방법}}

</details>

### 라이선스

이 프로젝트는 MIT 라이선스를 따릅니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참고하세요.

```
Copyright (c) {{YEAR}} {{AUTHOR}}
```

<!-- 의존성 라이선스 고지가 필요한 경우 -->
서드파티 라이선스 고지: [NOTICE](NOTICE)

---

<!-- ========== 7. 마무리 ========== -->
## 마무리

### 기여자

이 프로젝트에 기여해주신 모든 분들께 감사드립니다.

<a href="https://github.com/{{OWNER}}/{{REPO}}/graphs/contributors">
  <img src="https://contrib.rocks/image?repo={{OWNER}}/{{REPO}}" alt="contributors" />
</a>

### 감사의 말

- [{{참고 프로젝트}}]({{URL}}) — {{어떤 영감/코드를 받았는지}}
- [{{라이브러리}}]({{URL}}) — {{역할}}
- {{도움을 준 사람이나 조직}}

### 후원

이 프로젝트가 도움이 되었다면 ⭐️ 를 눌러주세요!

- [GitHub Sponsors](https://github.com/sponsors/{{OWNER}})
- [Open Collective](https://opencollective.com/{{PROJECT}})
- [Buy Me a Coffee](https://buymeacoffee.com/{{OWNER}})

### 관련 프로젝트

- [{{관련 프로젝트 1}}]({{URL}}) — {{설명}}
- [{{플러그인/확장}}]({{URL}}) — {{설명}}
- [{{공식 통합}}]({{URL}}) — {{설명}}

### 커뮤니티 및 연락처

- 💬 [Discord]({{DISCORD_URL}}) — 실시간 질문과 잡담
- 🗣 [GitHub Discussions](https://github.com/{{OWNER}}/{{REPO}}/discussions) — 아이디어 제안, Q&A
- 🐛 [Issues](https://github.com/{{OWNER}}/{{REPO}}/issues) — 버그 신고
- 🐦 [@{{HANDLE}}](https://twitter.com/{{HANDLE}})
- 📧 {{EMAIL}}

### 보안 취약점 신고

보안 취약점은 **공개 이슈로 등록하지 마시고** [SECURITY.md](SECURITY.md)의 절차에 따라 비공개로 제보해주세요.

---

<div align="center">

**[⬆ 맨 위로](#{{project_name}})**

Made with ❤️ by [{{AUTHOR}}]({{URL}})

</div>

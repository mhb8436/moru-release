<p align="center">
  <img src="images/brand/package-3d.png" width="300" alt="MORU 공공포털 플랫폼 v1.1">
</p>

<h1 align="center">표준프레임워크 사업, 누리집은 이미 만들어 두었습니다</h1>

<p align="center">
  전자정부 표준프레임워크 5.0으로 만든 누리집 CMS와 통합검색, 문서 AI, 위원회 업무 팩입니다.<br>
  환경변수를 하나도 건드리지 않아도 그대로 뜨고, AI를 쓰지 않는 사업이면 꺼 두면 됩니다.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/eGovFrame-5.0-0e2a47" alt="eGovFrame 5.0">
  <img src="https://img.shields.io/badge/KRDS-1.1-0e2a47" alt="KRDS 1.1">
  <img src="https://img.shields.io/badge/Spring%20Boot-3.5-0e2a47" alt="Spring Boot 3.5">
  <img src="https://img.shields.io/badge/Java-17-0e2a47" alt="Java 17">
  <img src="https://img.shields.io/badge/DB-PostgreSQL%20%7C%20MariaDB%20%7C%20Oracle-e8a020" alt="DB">
  <img src="https://img.shields.io/badge/%EC%8B%9C%ED%97%98-core%20139%20%C2%B7%20ai%20119%20%C2%B7%20UI%2070-1f6f4a" alt="시험">
  <img src="https://img.shields.io/badge/KRDS%20React-45%EB%B6%80%ED%92%88%20%C2%B7%20MIT-1f6f4a" alt="KRDS React 45컴포넌트 MIT">
  <img src="https://img.shields.io/badge/v1.1-2026--08-5a6b80" alt="v1.1">
</p>

<p align="center">
  <a href="https://mhb8436.github.io/moru-release/">제품 페이지</a> ·
  <a href="https://github.com/mhb8436/moru-release/releases/download/v1.1/MORU-brochure-v1.1.pdf">제품 소개서 PDF (A4 10쪽)</a> ·
  <a href="https://github.com/mhb8436/moru-release/releases/download/v1.1/MORU-leaflet-v1.1.pdf">리플릿 (A4 앞뒤)</a> ·
  <a href="https://github.com/mhb8436/moru-release/releases/download/v1.1/MORU-slides-v1.1.pptx">발표 자료 (PPTX 16장)</a> ·
  <a href="https://github.com/mhb8436/moru-release/releases/download/v1.1/MORU-demo-v1.1.mp4">시연 영상 (mp4 1분 59초)</a> ·
  <a href="https://github.com/mhb8436/moru-krds-react">KRDS React 컴포넌트 45종 (MIT)</a> ·
  <a href="#도입-문의">도입 문의</a>
</p>

---

## 데모

▶ **시연 영상(1분 59초, mp4)** — 아래 일곱 장면이 차례로 나옵니다. 장면마다 제목을 먼저 띄우고 아래쪽에 자막을 깔았습니다. [내려받기](https://github.com/mhb8436/moru-release/releases/download/v1.1/MORU-demo-v1.1.mp4) · [제품 페이지에서 바로 보기](https://mhb8436.github.io/moru-release/#demo)

가상 기관 ‘국립문서정보연구원’의 시연 데이터(문서 9건)를 넣고 로컬에서 찍었습니다. 손댄 곳 없이 실제로 돌아가는 화면 그대로입니다.

<table>
  <tr>
    <td width="50%"><img src="gifs/01-search.gif" alt="통합검색"><br><b>통합검색</b> — 게시물과 기관 문서 본문을 한 번에 찾습니다. 찾은 말은 노란색으로 짚어 줍니다.</td>
    <td width="50%"><img src="gifs/02-doc-ai.gif" alt="문서 AI"><br><b>문서 AI</b> — LLM 키를 넣지 않은 추출 모드입니다. 답변 문장마다 「근거 확인」 표시와 출처 번호가 붙습니다.</td>
  </tr>
  <tr>
    <td><img src="gifs/04-content.gif" alt="콘텐츠 승인·게시"><br><b>콘텐츠 승인 → 게시</b> — 초안을 올려 승인을 받고 게시하면 누리집에 바로 뜹니다. 저장할 때마다 버전이 남습니다.</td>
    <td><img src="gifs/03-committee.gif" alt="위원회 의결서"><br><b>위원회 의결서</b> — 회의 결과와 표수, 의결서를 함께 공개합니다. 의결서는 해시로 봉인해 두어, 열 때마다 「위변조 확인: 이상 없음」을 보여 줍니다.</td>
  </tr>
  <tr>
    <td><img src="gifs/06-security.gif" alt="보안 점검"><br><b>보안 점검</b> — 설정값을 읽어 판정합니다. CSRF와 비밀번호 정책, 보안 헤더, 오류 노출, CORS 다섯 가지는 서버가 자기 자신에게 요청을 보내 직접 재 봅니다.</td>
    <td><img src="gifs/05-language.gif" alt="언어 전환"><br><b>한국어 ↔ English</b> — 메뉴와 게시판 이름, 사이트 문구는 번역 표에서 관리하고 콘텐츠는 언어마다 따로 씁니다. 그 언어로 쓴 글이 없으면 기본 언어로 보여 줍니다.</td>
  </tr>
</table>

## 제품 구성

표준프레임워크는 프레임워크일 뿐, 그대로 쓸 수 있는 제품은 아닙니다. 그래서 사업마다 계정과 권한, 게시판, 첨부, 표준사전, 배치를 처음부터 다시 만들어 왔습니다. MORU는 그 일을 미리 해 둔 제품입니다. 이름은 대장간에서 달군 쇠를 올려놓고 두드리는 받침쇠 ‘모루’에서 따왔습니다.

| 구성 | 제공 기능 |
|---|---|
| **core** | 계정·인증(잠금·임시 비밀번호) · 권한 RBAC(게시판별 읽기/쓰기 역할) · 조직·사용자 · 게시판 엔진 · 첨부(확장자·MIME·시그니처 3중 검사, ClamAV) · 코드·표준사전(DDL 컬럼명 검증) · 배치 스케줄러 · 감사로그(해시 체인) · 알림(포털·메일·SMS) · 연계 어댑터 |
| **portal** | KRDS(디지털정부서비스 UI/UX 가이드라인) 누리집 틀(정부24와 같은 상단·주메뉴, 하위 페이지는 현재 경로+왼쪽 메뉴, 푸터) · 메뉴·IA · 콘텐츠(승인·버전·복원) · 회원(약관 이력·본인확인 연계점) · 템플릿(기관명·테마·레이아웃을 데이터로 관리) · 팝업·배너 · KRDS React 컴포넌트 45종(별도 공개) · 통합검색 · 개방 API(X-API-Key·일일 한도·OpenAPI 3.0) · 웹로그 통계 · 관리자 접근통제(IP·TOTP) |
| **ai** | AI 게이트웨이(개인정보 마스킹·쿼터·서킷브레이커·DMZ 중계) · 문서 파싱(HWP·HWPX·HWPML·PDF·DOCX·XLSX·CSV·TXT·MD·JSON) · 색인·검색(BM25·벡터·RRF) · 챗봇(멀티턴·시나리오·콘텐츠 초안) · 근거 검증(문장↔출처) |
| **게시판 유형** | 공지 · FAQ · 자료실 · 포토갤러리 · 묻고 답하기 · 동영상 · E-Book |
| **업무 팩 — 위원회** | 위원회·위원·회의·안건·표결·의결서 관리. 정족수 비율, 법정기한(소집 통지 7일·안건 송부 3일), 가부동수 규칙, 서면의결 이중 정족수, 의결서 해시 봉인 |
| **관리자** | 배치 · 사용자·권한 · 조직 · 감사로그 · 접속로그 · 코드 · 표준사전 · 게시판 정의 · 메뉴 · 콘텐츠 · 사이트·템플릿 · 팝업·배너 · 접속 통계 · 개방 API · AI · 필터링 단어 · SMS · 알림 · 위원회 · 보안 점검 |

## 화면을 컴포넌트로 조립합니다

누리집도 관리 화면도 KRDS 규격에 맞춘 React 컴포넌트 45종으로 조립합니다. 화면마다 마크업을 새로 짜지 않으니 기관이 화면을 늘려도 접근성과 디자인 규격을 화면마다 따로 챙기지 않아도 됩니다. portal 안에서 이 컴포넌트를 가져다 쓰는 자리가 82곳입니다.

| 묶음 | 컴포넌트 |
|---|---|
| **누리집 틀** 9 | 머리표시 · 헤더 · 주메뉴 · 이동경로 · 왼쪽 메뉴 · 페이지 내 목차 · 푸터 · 기관 식별자 · 건너뛰기 링크 |
| **입력** 10 | 필드 · 텍스트 입력 · 여러 줄 입력 · 선택 · 체크박스 · 라디오 · 파일 올리기 · 콤보박스 · 입력 그룹 · 단추 |
| **자료** 5 | 표 · 데이터 표(정렬 · 머리 고정 · 빈 상태) · 정의 목록 · 글 목록 · 페이지 이동 |
| **상태** 9 | 인라인 경고 · 긴급 경고 · 토스트 · 빈 상태 · 스켈레톤 · 스피너 · 진행 막대 · 배지 · 태그 |
| **겹침** 4 | 모달 · 드로어 · 툴팁 · 컨텍스트 메뉴 |
| **펼침** 4 | 탭 · 아코디언 · 접기 · 단계 표시 |
| **그 밖에** 4 | 아바타 · 구분선 · 스크롤 영역 · 글씨 크기 조절 |

- **KRDS에 없는 13종은 직접 그렸습니다.** 드로어 · 토스트 · 콤보박스 · 컨텍스트 메뉴 · 정렬되는 데이터 표처럼 관리 화면에는 있어야 하지만 킷에는 없는 컴포넌트입니다. KRDS 토큰만 써서 만들었으니 나머지와 섞어 놓아도 표가 나지 않습니다.
- **관리 화면 11개는 뼈대가 같습니다.** 목록에서 「등록」을 누르면, 입력칸이 10개가 넘는 화면은 화면 자체가 바뀌고 그보다 적으면 모달이 열립니다. 화면마다 다르게 만들지 않았으니 담당자가 탭을 옮겨 다녀도 쓰는 방법이 같습니다.
- **45종 가운데 31종은 서버에서 그립니다.** 목록이나 본문처럼 첫 화면에 바로 보여야 하는 것은 브라우저가 자바스크립트를 받을 때까지 기다리지 않습니다.
- **컴포넌트 문서 화면이 제품 안에 있습니다.** `/ui`에 컴포넌트마다 한 줄 설명과 예제, 코드, 「이럴 때 쓴다 · 이럴 때 쓰지 않는다」, 변형, 속성 표를 적어 두었습니다. 왼쪽 목록도 이 라이브러리의 컴포넌트로 만들었습니다.

<p align="center">
  <img src="images/screens/15-컴포넌트문서.jpg" width="900" alt="컴포넌트 문서 화면 — Button">
  <br><sub>제품에 들어 있는 컴포넌트 문서 화면입니다. 컴포넌트마다 예제와 코드, 「이럴 때 쓴다 · 이럴 때 쓰지 않는다」, 변형, 속성 표가 붙습니다.</sub>
</p>

## 컴포넌트 라이브러리 — moru-krds-react

45종은 MORU 없이도 쓸 수 있도록 따로 떼어 **MIT 라이선스**로 공개했습니다.
[github.com/mhb8436/moru-krds-react](https://github.com/mhb8436/moru-krds-react) · [npm](https://www.npmjs.com/package/moru-krds-react)

```bash
npm i krds-uiux moru-krds-react
```

```tsx
import 'krds-uiux/resources/cdn/krds.min.css';
import { Field, TextInput, Button } from 'moru-krds-react';

<Field id="name" label="이름" required hint="공백 없이 적어 주세요">
  {(a) => <TextInput {...a} value={name} onChange={onChange} />}
</Field>
<Button variant="primary">신청하기</Button>
```

- **KRDS 킷은 넣지 않았습니다.** krds.min.css와 글꼴은 공식 배포판 `krds-uiux`를 그대로 받아 씁니다. 망분리 환경이면 `resources/`를 정적 폴더에 복사해 두고 씁니다.
- **프레임워크를 가리지 않습니다.** 프레임워크에 닿는 자리가 `lib/link.tsx` 한 곳뿐이라, Next.js든 React Router든 맨 `<a>`든 그 파일만 바꾸면 섭니다.
- **Tailwind를 쓰신다면** `styles/krds-tailwind.css`를 같이 불러오십시오. `text-fg-subtle` 같은 이름을 KRDS 변수에 이어 줍니다. 불러오지 않아도 컴포넌트는 그대로 돌아갑니다.
- **규칙은 소스에 적어 두었습니다.** 컴포넌트마다 파일 머리에 무엇을 지켜야 하는지, 무엇을 하면 안 되는지 써 두었습니다.

## 구조

```mermaid
flowchart LR
  U[국민 · 담당자<br>브라우저] --> P
  P[MORU portal<br>Next.js · TypeScript<br>:3000] --> C
  C[MORU core<br>표준프레임워크 5.0 · Spring Boot 3.5<br>Tomcat 10 · Java 17 · MyBatis · Flyway<br>:8080] --> DB[(PostgreSQL · H2<br>MariaDB · Oracle)]
  C -. 선택 .-> A[MORU ai<br>FastAPI :8800]
  A --> S[색인 SQLite+BM25<br>→ OpenSearch · Elasticsearch]
  A --> V[벡터 미사용<br>→ pgvector · kNN]
  A --> L[LLM 미사용<br>→ Ollama · vLLM · OpenAI 규격]
```

환경변수를 하나도 건드리지 않아도 `./deploy/run.sh` 한 번이면 프로세스 세 개가 뜹니다. 이때는 H2 파일과 SQLite+BM25, Kiwi를 씁니다. 도커도, 따로 사 와야 하는 소프트웨어도 없습니다.

| 층 | 기본 | 기관 요구가 있을 때 |
|---|---|---|
| DB | PostgreSQL (운영) · H2 (로컬) | MariaDB · Oracle/Tibero (Flyway 벤더 폴더 + MyBatis `databaseId`) |
| 검색 | SQLite + BM25 | OpenSearch(nori) · Elasticsearch |
| 벡터 | 사용하지 않음 | pgvector · sqlite-vec · OpenSearch kNN, 임베딩은 `/v1/embeddings` 규격 |
| LLM | 사용하지 않음 (추출 모드) | OpenAI 호환 엔드포인트 |
| 형태소 | Kiwi | Nori — 표준용어 사전을 양쪽 사용자 사전으로 공유 |

## 화면

<table>
  <tr>
    <td><img src="images/screens/01-메인.jpg" alt="누리집 메인"></td>
    <td><img src="images/screens/03-문서AI.jpg" alt="문서 AI"></td>
  </tr>
  <tr>
    <td><img src="images/screens/11-관리자-보안점검.jpg" alt="관리자 보안 점검"></td>
    <td><img src="images/screens/10-관리자-표준사전.jpg" alt="관리자 표준사전"></td>
  </tr>
</table>

## 도입 · 문의

- **도입 형태** — 기관 서버에 설치해 씁니다. 프로세스 세 개를 한 대에 몰아 두어도 되고, 세 대로 나누어도 됩니다. AWS·Azure 같은 클라우드 계정은 필요 없고, 제품이 도는 데 바깥 서비스를 부르지 않습니다. 밖으로 나가는 연결은 기관이 켠 것뿐입니다 — LLM, 문자(SENS), 본인확인, 동영상 게시판의 유튜브 썸네일.
- **망분리 환경** — AI 사이드카를 빼고 core와 portal만 돌려도 되고, LLM 호출만 DMZ의 squid로 내보내도 됩니다.
- **시작하기** — 비어 있는 PostgreSQL 하나와 환경변수 여섯 개면 됩니다. 처음 뜰 때 Flyway가 테이블 36개를 만듭니다. 자세한 절차는 [제품 소개서](docs/MORU-제품소개서-v1.1.pdf) 10쪽에 있습니다.
- **문의** — 주식회사 크래프틱시스템즈. 이 저장소 [Issues](../../issues)에 남겨 주시거나 아래 연락처로 연락 주십시오.
  - 전자우편: mhb8436@gmail.com

## In English

MORU is an on-premises public-portal product built on the Korean eGovFrame 5.0 runtime with the KRDS (Korea Design System) portal shell (Spring Boot 3.5 · Tomcat 10 · Java 17). It ships with accounts, RBAC, boards, attachments, a standard-term dictionary, batch jobs, hash-chained audit logs, a CMS with approval and versioning, unified search, and a document-AI sidecar that reads HWP/HWPX/HWPML without external libraries and attaches evidence to every answer sentence. It runs with zero configuration (H2 · SQLite BM25 · Kiwi) and switches to PostgreSQL/MariaDB/Oracle, OpenSearch, pgvector and any OpenAI-compatible LLM through environment variables. The LLM can be turned off entirely. Its 45 KRDS React components — the ones every public and admin screen is assembled from — are released separately under MIT as [moru-krds-react](https://github.com/mhb8436/moru-krds-react).

---

<p align="center">
  <img src="images/brand/logo-horizontal.png" width="220" alt="MORU"><br>
  <sub>이 저장소의 이미지와 문서는 주식회사 크래프틱시스템즈의 저작물이고, 제품을 소개하려고 공개합니다. 소스 코드는 다른 저장소에서 관리합니다.</sub>
</p>

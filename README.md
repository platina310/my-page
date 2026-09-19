https://github.com/platina310/my-page

# 개인 과제 — 개인 소개 페이지 + 프론트엔드·백엔드 연동

DFMBA 클라우드컴퓨팅실습 개인 과제 저장소입니다.

## 프로젝트 소개

HTML·CSS·JavaScript로 만든 개인 소개 페이지와, React 화면에서 FastAPI 백엔드 API를 호출해
메모를 저장·조회·삭제하는 풀스택 메모 앱으로 구성되어 있습니다.
소개 페이지의 링크로 메모 앱(연동 실습 페이지)에 접근할 수 있고, 메모 앱에서도 소개 페이지로 돌아올 수 있습니다.

## 주요 구성

| 구분 | 기술 | 배포 | 소스 코드 |
|---|---|---|---|
| 개인 소개 페이지 | HTML · CSS · JavaScript | Vercel | 이 저장소 (`index.html`, `style.css`, `script.js`) |
| 프론트엔드 (메모 앱 화면) | React (Vite) | Vercel | https://github.com/platina310/memo-frontend |
| 백엔드 (메모 API) | FastAPI · SQLAlchemy | Render | 메모백엔드_저장소_주소https://github.com/platina310/memo-backend |
| 데이터베이스 | PostgreSQL | Supabase | - |

동작 흐름

1. 브라우저가 Vercel에서 메모 앱 화면을 받는다.
2. 화면이 `fetch`로 Render의 FastAPI 엔드포인트(`GET/POST/DELETE /memos`)를 호출한다.
3. FastAPI가 Supabase(PostgreSQL)에 메모를 저장·조회하고 JSON으로 응답한다.
4. 화면이 응답을 받아 메모 목록을 다시 그린다.

소개 페이지 기능: 프로필 카드, 관심 분야 태그, 경력 타임라인, 다크모드 전환, 모바일 대응

## 배포 주소

- 개인 소개 페이지: https://my-page-dfmba.vercel.app
- 연동 실습 페이지(메모 앱): https://memo-frontend-dfmba.vercel.app
- 백엔드 Swagger UI: https://memo-backend-3iqc.onrender.com/docs

> Render 무료 플랜은 일정 시간 요청이 없으면 휴면 상태가 되어, 첫 접속 시 30초~1분 정도 걸릴 수 있습니다.
https://github.com/platina310/my-page

# 개인 과제 — 개인 소개 페이지 + 프론트엔드·백엔드 연동

## 프로젝트 소개
HTML/CSS/JS로 만든 개인 소개 페이지와, React 프론트엔드에서
FastAPI 백엔드 API를 호출해 메모를 저장·조회·삭제하는 풀스택 메모 앱입니다.

## 주요 구성
| 구분 | 기술 | 배포 | 저장소 |
|---|---|---|---|
| 개인 소개 페이지 | HTML · CSS · JS | Vercel | 이 저장소 |
| 프론트엔드 | React (Vite) | Vercel | https://github.com/<사용자명>/memo-frontend |
| 백엔드 | FastAPI · SQLAlchemy | Render | https://github.com/<사용자명>/memo-backend |
| 데이터베이스 | PostgreSQL | Supabase | - |

흐름: 소개 페이지 → (링크) → 메모 앱 → fetch → FastAPI → PostgreSQL

## 배포 주소
- 개인 소개 페이지: https://my-page-dfmba.vercel.app
- 연동 실습(메모 앱): https://memo-frontend-dfmba.vercel.app
- 백엔드 Swagger UI: https://memo-backend-3iqc.onrender.com/docs
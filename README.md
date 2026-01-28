# 카드 뒤집기 게임

HTML/CSS/JS + Supabase 기반 메모리 카드 게임.

## 로컬 실행

1. `config.example.js` 를 `config.js` 로 복사한다.
2. Supabase 프로젝트의 **URL**, **anon key** 를 `config.js` 에 넣는다.
3. `index.html` 을 브라우저로 연다 (또는 `npx serve .` 등 로컬 서버 사용).

`config.js` 는 `.gitignore` 대상이므로 저장소에 포함되지 않는다. 키 유출을 막기 위해 반드시 분리해 두었다.

## 배포

Vercel, Netlify, GitHub Pages 등 정적 호스팅에 올린 뒤, 해당 서비스에서 환경 변수로 Supabase URL·anon key 를 넣고 **빌드 시 `config.js` 를 생성**하는 방식으로 설정한다.  
(또는 배포 환경에 `config.js` 를 직접 업로드하되, 해당 파일은 Git 에 넣지 않는다.)

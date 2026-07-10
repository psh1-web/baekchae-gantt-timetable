# 백채CIC 고도화전략 실행 타임테이블

## 파일 구조
```
├── index.html    ← 간트차트 UI
├── data.json     ← 일정·진척률 데이터 (수정 시 이 파일만 변경됨)
├── vercel.json   ← Vercel 설정
└── README.md
```

## Vercel 배포 방법
1. GitHub에 이 폴더 내용을 올립니다
2. vercel.com 접속 → New Project → GitHub 저장소 연결
3. Framework = Other, Root Directory = / 로 설정
4. Deploy → URL 생성 완료

## 데이터 자동 업데이트 방법
1. 브라우저에서 간트차트 URL 접속
2. **⚙ GitHub 설정** 버튼 클릭
   - Owner/Repo: `본인아이디/저장소명` 입력
   - Token: GitHub Personal Access Token (repo 권한) 입력
   - 설정 저장
3. 일정·진척률 수정 후 **↑ 저장 (GitHub Push)** 버튼 클릭
4. Vercel이 자동 재배포 (약 30초) → 모든 접속자에게 반영

## GitHub Token 발급
GitHub → Settings → Developer settings → Personal access tokens → Generate new token  
권한: `repo` 체크 (Full control of private repositories)

> ⚠️ Token은 본인 브라우저에만 저장되며 서버로 전송되지 않습니다.

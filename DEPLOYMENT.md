# SMCP Verbs 100 배포 가이드

이 가이드는 SMCP Verbs 100 앱을 GitHub과 Netlify를 통해 배포하는 단계별 절차를 제공합니다.

## 사전 준비사항

- Git이 설치되어 있어야 합니다
- GitHub 계정 (sirius4600)
- 인터넷 연결

## 1단계: Git 저장소 초기화

프로젝트 폴더에서 명령 프롬프트를 열고 다음 명령어를 실행하세요:

```bash
# 프로젝트 폴더로 이동
cd C:\Users\kathe\Desktop\pilot\smcpv100

# Git 저장소 초기화
git init

# 모든 파일 추가
git add .

# 첫 번째 커밋
git commit -m "Initial commit: SMCP Verbs 100 learning app"
```

## 2단계: GitHub 저장소 생성

1. https://github.com에 로그인
2. 우측 상단 "+" 버튼 클릭 → "New repository"
3. Repository name: `smcp-verbs-100`
4. Description: `표준해사통신용어 핵심 동사 100개 학습 앱`
5. Public 선택
6. "Create repository" 클릭

## 3단계: GitHub에 코드 업로드

```bash
# 원격 저장소 추가
git remote add origin https://github.com/sirius4600/smcp-verbs-100.git

# 기본 브랜치를 main으로 설정
git branch -M main

# GitHub에 푸시
git push -u origin main
```

## 4단계: Netlify 배포

### 4-1. Netlify 계정 생성/로그인
1. https://netlify.com 접속
2. "Sign up" 또는 "Log in"
3. GitHub 계정으로 로그인 선택

### 4-2. 새 사이트 배포
1. 대시보드에서 "Add new site" → "Import an existing project"
2. "Deploy with GitHub" 선택
3. GitHub 계정 연결 승인
4. `smcp-verbs-100` 저장소 선택
5. 배포 설정:
   - **Branch to deploy**: main
   - **Build command**: 비워두기
   - **Publish directory**: 비워두기
6. "Deploy site" 클릭

## 5단계: 배포 확인

배포가 완료되면 Netlify가 임시 URL을 제공합니다:
- 형태: `https://wonderful-app-123456.netlify.app`

### 테스트 항목
- [ ] 앱이 정상적으로 로드되는지 확인
- [ ] 다크/라이트 모드 토글 기능
- [ ] 카드 클릭으로 답안 표시
- [ ] 진행률 바 업데이트
- [ ] 이전/다음 버튼 기능
- [ ] 키보드 단축키 (스페이스바, 화살표 키)
- [ ] 모바일에서 터치 동작
- [ ] 완료 화면 표시

## 6단계: 사이트 이름 변경 (선택사항)

1. Netlify 대시보드에서 사이트 선택
2. "Site settings" → "Change site name"
3. 원하는 이름으로 변경 (예: `smcp-verbs-100`)
4. 최종 URL: `https://smcp-verbs-100.netlify.app`

## 자동 배포 설정

GitHub에 새로운 변경사항을 푸시할 때마다 Netlify가 자동으로 재배포됩니다:

```bash
# 파일 수정 후
git add .
git commit -m "Update: 설명"
git push
```

## 문제 해결

### 배포 실패 시
1. Netlify의 "Deploys" 탭에서 로그 확인
2. 파일 경로와 이름이 정확한지 확인
3. index.html이 루트 디렉토리에 있는지 확인

### 한국어 텍스트가 깨질 때
- index.html의 `<meta charset="UTF-8">` 확인
- 파일이 UTF-8로 저장되었는지 확인

### 모바일에서 스타일이 깨질 때
- 브라우저 캐시 새로고침 (Ctrl+F5)
- 다른 모바일 브라우저에서 테스트

## 추가 설정

### 사용자 정의 도메인
1. 도메인을 소유하고 있다면 Netlify에서 사용자 정의 도메인 설정 가능
2. "Domain settings" → "Add custom domain"

### HTTPS 자동 설정
- Netlify는 자동으로 SSL 인증서를 제공하여 HTTPS 지원

### 분석 도구 연결
- Google Analytics나 기타 분석 도구 연결 가능

## 완료

배포가 성공적으로 완료되면:
- 전 세계 어디서나 URL로 접속 가능
- 모바일/데스크톱 모든 기기에서 동작
- 자동 배포로 업데이트 간편
- 무료 호스팅으로 비용 부담 없음

축하합니다! SMCP Verbs 100 앱이 성공적으로 배포되었습니다.
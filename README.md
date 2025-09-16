# SMCP Verbs 100

표준해사통신용어(Standard Marine Communication Phrases) 핵심 동사 100개를 학습할 수 있는 웹 애플리케이션입니다.

## 🚢 소개

SMCP Verbs 100은 해사 관련 업무에 필수적인 영어 동사 100개를 효율적으로 학습할 수 있도록 설계된 플래시카드 앱입니다. 모바일과 데스크톱 모두에서 최적화되어 언제 어디서나 학습할 수 있습니다.

## ✨ 주요 기능

- **100개의 핵심 동사**: 중요도 순으로 정렬된 표준해사통신용어 동사
- **인터랙티브 학습**: 카드를 클릭하여 답안 확인
- **진행률 추적**: 실시간 학습 진행률 표시
- **다크/라이트 모드**: 사용자 선호에 따른 테마 선택
- **모바일 최적화**: 반응형 디자인으로 모든 기기에서 완벽 지원
- **키보드 지원**: 스페이스바, 화살표 키를 이용한 편리한 조작
- **학습 통계**: 완료 시 학습 시간 및 성과 표시

## 🎮 사용 방법

1. **카드 클릭**: 한국어 문제 카드를 클릭하면 영어 답안이 표시됩니다
2. **다음 문제**: 답안이 표시된 상태에서 다시 클릭하면 다음 문제로 넘어갑니다
3. **이전 문제**: "← 이전" 버튼으로 이전 문제로 돌아갈 수 있습니다
4. **테마 변경**: 우측 상단의 ☀️/🌙 버튼으로 다크/라이트 모드를 전환할 수 있습니다

### 키보드 단축키
- `스페이스바` 또는 `엔터`: 답안 보기 / 다음 문제
- `←` (왼쪽 화살표): 이전 문제
- `→` (오른쪽 화살표): 다음 문제 (답안이 표시된 상태에서만)

## 🛠 기술 스택

- **HTML5**: 시맨틱 마크업과 접근성
- **CSS3**: 모던 스타일링과 애니메이션
  - CSS Variables (Custom Properties)
  - Flexbox & Grid Layout
  - Media Queries (반응형 디자인)
  - CSS Animations
- **Vanilla JavaScript**: 가벼운 인터랙션과 상태 관리
- **Progressive Web App**: 모바일 최적화 및 오프라인 지원

## 📱 호환성

- **모바일**: iOS Safari, Android Chrome
- **데스크톱**: Chrome, Firefox, Safari, Edge
- **태블릿**: iPad, Android 태블릿
- **반응형**: 320px 이상의 모든 화면 크기 지원

## 🚀 배포

이 앱은 정적 웹사이트로 구축되어 다음 플랫폼에 쉽게 배포할 수 있습니다:

- **Netlify**: 권장 배포 플랫폼
- **Vercel**: 대안 배포 플랫폼
- **GitHub Pages**: 무료 호스팅
- **Firebase Hosting**: Google 플랫폼

### Netlify 배포 방법

1. 이 저장소를 GitHub에 푸시
2. [Netlify](https://netlify.com)에서 "New site from Git" 선택
3. GitHub 저장소 연결
4. 자동 배포 완료

## 📚 학습 내용

앱에 포함된 100개의 동사는 다음과 같은 해사 상황에서 자주 사용됩니다:

- 선박 조종 및 운항
- 응급상황 대응
- 화물 적재/하역
- 항만 작업
- 안전 관리
- 통신 및 보고

## 🔧 개발자를 위한 정보

### 프로젝트 구조
```
smcpv100/
├── index.html          # 메인 애플리케이션 파일
├── README.md           # 프로젝트 문서
└── .gitignore         # Git 무시 파일 목록
```

### 개발 환경 설정
```bash
# 저장소 클론
git clone https://github.com/sirius4600/smcp-verbs-100.git

# 프로젝트 폴더로 이동
cd smcp-verbs-100

# 로컬 서버로 실행 (Python 3)
python -m http.server 8000

# 브라우저에서 접속
# http://localhost:8000
```

### 커스터마이징

동사 목록을 수정하려면 `index.html` 파일의 JavaScript 부분에서 `verbs` 배열을 편집하세요:

```javascript
const verbs = [
    {rank: 1, korean: "보관하다, 잡다", english: "hold"},
    {rank: 2, korean: "위치하다", english: "stand"},
    // ... 추가 동사들
];
```

## 📄 라이센스

이 프로젝트는 MIT 라이센스 하에 제공됩니다. 자유롭게 사용, 수정, 배포할 수 있습니다.

## 🤝 기여하기

버그 리포트, 기능 제안, 풀 리퀘스트를 환영합니다!

1. 이 저장소를 포크합니다
2. 새로운 기능 브랜치를 생성합니다 (`git checkout -b feature/새기능`)
3. 변경사항을 커밋합니다 (`git commit -am '새 기능 추가'`)
4. 브랜치에 푸시합니다 (`git push origin feature/새기능`)
5. 풀 리퀘스트를 생성합니다

## 📞 연락처

문의사항이나 제안이 있으시면 GitHub Issues를 통해 연락해 주세요.

---

⚓ **Happy Learning!** 표준해사통신용어 마스터가 되어보세요!
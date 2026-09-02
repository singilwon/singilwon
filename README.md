<p align="center">
<img width="1524" height="350" alt="Profile Banner" src="https://github.com/user-attachments/assets/e8d88cf4-7b4b-4d16-8063-161eca656180" />
</p>

<p align="center">
사용자 흐름을 이해하고, 기능 구현 이후의 구조와 유지보수성까지 함께 고민하는 프론트엔드 개발자입니다.
</p>

<p align="center">
<img src="https://media.giphy.com/media/l3vR85PnGsBwu1PFK/giphy.gif" width="220"/>
</p>

<p align="center">
<i>"사용자와 가장 가까운 화면에서 더 나은 경험을 만드는 개발자를 지향합니다."</i>
</p>

---

# 🕸 About Me

사용자와 가장 가까운 영역에서 문제를 해결할 수 있다는 점에 매력을 느껴  
프론트엔드 개발을 공부하고 있습니다.

React와 Next.js 기반 프로젝트를 진행하며  
단순히 화면을 구현하는 것에서 끝나지 않고,  
**상태 관리, API 연동, 컴포넌트 구조, 예외 상황 처리**까지 함께 고민하고 있습니다.

관심 있는 분야는 다음과 같습니다.

- 사용자 흐름을 고려한 UI 구현
- 상태 관리와 서버 데이터 동기화
- 유지보수성을 고려한 컴포넌트 설계
- 기능 책임 분리와 리팩토링
- 실제 사용자 입력과 상호작용 문제 해결

---

# 🛠 Tech Stack

<p align="center">
<img src="https://skillicons.dev/icons?i=js,ts,react,nextjs,tailwind,supabase,git,github,figma,vercel,html,css"/>
</p>

<p align="center">
<img src="https://img.shields.io/badge/Zustand-443E38?style=for-the-badge&logoColor=white"/>
<img src="https://img.shields.io/badge/TanStack_Query-FF4154?style=for-the-badge&logo=reactquery&logoColor=white"/>
<img src="https://img.shields.io/badge/Axios-5A29E4?style=for-the-badge&logo=axios&logoColor=white"/>
<img src="https://img.shields.io/badge/REST_API-02569B?style=for-the-badge&logoColor=white"/>
<img src="https://img.shields.io/badge/CSS_Modules-000000?style=for-the-badge&logo=cssmodules&logoColor=white"/>
</p>

---

# 🚀 Featured Projects

## ⚡ BuzzerBidder

Next.js 기반의 경매형 중고 거래 서비스입니다.  
실시간 경매와 일반 경매를 통해 상품을 거래하고, 서비스 내 재화인 Bizz를 활용해 결제 흐름을 제공합니다.

### 주요 기능

- Toss Payments 기반 코인(Bizz) 충전
- 거래 상세 페이지
- 구매자 / 판매자 역할별 거래 정보 분기
- 구매 확정 처리
- 마이페이지 구매 / 판매 / 찜 목록 관리
- 찜 토글 기능

### 담당 역할

- 코인(Bizz) 충전 및 결제 승인 흐름 구현
- Toss Payments 결제 요청 / 승인 / 실패 처리 흐름 분리
- 결제 완료 / 실패 화면 공통 컴포넌트화
- 거래 상세 및 구매 확정 흐름 구현
- 마이페이지 상품 목록 UI 구현
- 찜 토글 UX 개선
- React Query query key 및 캐시 갱신 구조 개선

### 개선 경험

결제 성공 처리 과정에서 URL 파라미터 검증, 승인 API 호출, 결과 화면 표시 등 여러 책임이 한 흐름에 섞여 있었습니다.  
이를 결제 요청 로직, 성공 처리 컴포넌트, 파라미터 검증 hook, 결과 화면 컴포넌트로 분리하여 역할을 명확히 했습니다.

또한 React Query의 query key를 기능별로 정리하고,  
충전 / 거래 확정 / 찜 상태 변경 이후 필요한 데이터가 일관되게 갱신되도록 개선했습니다.

### Focus

- Next.js App Router
- Toss Payments 연동
- TanStack Query 기반 서버 상태 관리
- 결제 플로우 책임 분리
- 사용자 액션 이후 데이터 동기화
- 유지보수성을 고려한 컴포넌트 구조

---

## 🥔 Hot Potato

React 기반의 밸런스 게임 커뮤니티 서비스입니다.  
사용자가 밸런스 게임 게시글을 탐색하고, 투표·댓글·좋아요·신고·알림 기능을 통해 상호작용할 수 있습니다.

### 주요 기능

- 밸런스 게임 게시글 탐색
- 사용자 / 게시글 검색
- 투표, 댓글, 좋아요
- 신고 모달
- 알림 모달
- Empty State
- Skeleton UI
- 비속어 필터

### 담당 역할

- Header UI 및 페이지 이동 링크 구현
- 검색 페이지 전체 UI 구현
- 사용자 / 게시글 검색 Supabase 연동
- 검색어 하이라이트 및 최신순 정렬 구현
- 검색 결과 없음 UI 구현
- Sure / Report / Alarm 모달 구현
- 알림 삭제 및 모달 내부 클릭 동작 처리
- 신고 내용 글자 수 제한 및 Toast 피드백 처리
- 게시글 Empty State 및 Profile no post 화면 구현
- Skeleton UI 구현
- 게시물 비속어 필터 구현

### Troubleshooting

신고 모달 textarea에서 한글 입력 시 문자가 2번씩 입력되는 문제가 발생했습니다.

처음에는 React StrictMode의 중복 실행 문제를 의심했지만,  
StrictMode를 제거해도 문제가 해결되지 않았습니다.

이후 onChange 상태 업데이트와 IME composition 문제를 확인하기 위해  
입력 중 상태를 따로 관리하는 방식도 시도했지만 문제가 지속되었습니다.

최종적으로 중첩 모달 내부에서 Portal로 신고 모달을 띄우던 구조를 재검토했고,  
부모 페이지에서 신고 모달의 open 상태를 제어하도록 변경했습니다.

이를 통해 한글 중복 입력 문제와  
모달이 부모 영역 안에 갇히는 문제를 함께 해결했습니다.

### Focus

- 검색 UX
- Supabase 데이터 연동
- 사용자 피드백 모달
- Empty / Loading 상태 처리
- 커뮤니티 안전성 보완
- 사용자 입력 이슈 디버깅

---

# 📊 GitHub Stats

<p align="center">

<img height="165" src="https://github-readme-stats.vercel.app/api?username=singilwon&show_icons=true&theme=tokyonight&hide_border=true"/>

<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=singilwon&layout=compact&theme=tokyonight&hide_border=true"/>

</p>

---

# 📈 Activity Graph

<p align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=singilwon&theme=tokyo-night&hide_border=true"/>

</p>

---

# 🐍 Contribution Snake

<p align="center">

<img src="https://raw.githubusercontent.com/singilwon/output/github-contribution-grid-snake.svg"/>

</p>

---

# 📫 Contact

<p align="center">

<a href="mailto:joowoni98@gmail.com">
<img src="https://img.shields.io/badge/email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>

<a href="https://github.com/singilwon">
<img src="https://img.shields.io/badge/github-111111?style=for-the-badge&logo=github&logoColor=white"/>
</a>

</p>

---

<p align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&height=140&section=footer&color=0:0F172A,50:2563EB,100:0F172A"/>
</p>

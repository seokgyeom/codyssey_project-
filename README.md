# codyssey_project-
# 📱 FreshRoutine PRO — AI 기반 모바일 루틴 형성 서비스 UI/UX 디자인 프로젝트

> **현대적인 iOS 18 HIG 기반의 미니멀 인터페이스와 AI 가이드라인을 결합한 스마트 습관 형성 플랫폼**

---

## 1. 프로젝트 개요 (Project Overview)

* **서비스명**: FreshRoutine PRO (프레시루틴 프로)
* **플랫폼**: Mobile iOS (iPhone 16 Pro / 390×844 해상도 기준)
* **디자인 시스템**:
  * **Style**: Modern iOS 18 HIG 스타일, Clean & Minimalist UI
  * **Color Palette**: Pure White (`#FFFFFF`), Primary Teal (`#00C897` / `#1DB8A4`), Soft Slate (`#5B6E8A`), Mint Background (`#D4F5EF` / `#E0F5F3`), Dark Navy/Charcoal (`#0F172A`)
  * **Typography**: iOS System Font (San Francisco / Noto Sans KR)
* **산출물 링크**:
  * 🎨 **Figma 프로젝트 링크**: [Figma Prototype 바로가기](https://www.figma.com/make/fW04R1xQ1T4rV8gCoft5fu/Prototype-FreshRoutine-PRO-App?viewport=489%2C430%2C1&t=Xt4PEwS90sphVy2t-0)
  * 🌐 **배포 프로토타입 링크**: [Live Prototype 바로가기](https://chord-gold-33413710.figma.site/)

---

## 2. 핵심 UI/UX 디자인 시안 (Screens)

| 1. 온보딩 (진단 & 추천) | 2. 메인 대시보드 (오늘) | 3. 탐색 (가이드 & 템플릿) |
| :---: | :---: | :---: |
| 4단계 중 2단계 목표 진단 및 카드 선택 | 원형 진행률 위젯 및 블록별 루틴 체크리스트 | 앤드류 휴버먼 추천 배너 및 루틴 템플릿 목록 |

| 4. 새 루틴 만들기 (빌더) | 5. 리포트 (통계 & 스트릭) | 6. 마이페이지 (프로필 & 설정) |
| :---: | :---: | :---: |
| 가이드 연동, 요일/시간 및 목표 유형 설정 폼 | 14일 연속 달성 스트릭 및 월간 캘린더 잔디 통계 | 실천 가이드 배지, PRO 구독 관리 및 시스템 설정 |

| 7. 포커스 모드 (타이머) | 8. PRO 구독 & 결제 (페이월) |
| :---: | :---: |
| 집중 몰입 다크모드 및 펄스 원형 타이머 | AI 무제한 생성 혜택 안내 및 연간/월간 플랜 선택 |

---

## 3. 프롬프트 엔지니어링 및 작업 로그 (Work Log)

AI 이미지 생성 도구를 활용하여 일관된 디자인 시스템을 구축하고, 텍스트 깨짐 및 언어 불일치 문제를 해결해 나간 프롬프트 최적화 기록입니다.

| 화면 구분 | 단계 | 사용 프롬프트 (Prompt) | 결과 및 개선점 (Result & Reflection) |
| :--- | :---: | :--- | :--- |
| **새 루틴 만들기 (Builder)** | **초안** | `[Role] Senior Mobile App UI/UX Designer [Task] Design the Routine Builder screen for "FreshRoutine" [Design System] Clean Form, Pure White, Teal (#00C897) [Screen Content] Input Section 1: 루틴 이름...` | • 레이아웃과 폼 컴포넌트는 정상 생성되었으나 `Input Section`, `Schedule Picker` 등의 프롬프트 잔여 영문 텍스트가 라벨로 노출됨. |
| | **수정** | `[Task] Revise the existing "Create New Routine" screen... Only replace leftover English UI labels with Korean. Do not redesign. [Screen Content] 취소 / 새 루틴 만들기 / 저장, 루틴 이름, 연결 가이드라인, 반복 요일 [Do Not Include] Any English on screen, Prompt leftovers...` | • 프롬프트 불필요 텍스트 제거 및 한글 전용 라벨(`루틴 이름`, `연결 가이드라인`, `반복 요일`) 지정으로 완성도 향상. |
| | **최종** | `Photorealistic iPhone app UI mockup. Identical to the 1st version except Korean labels. Figma-ready UI design.` | • 완벽한 한글 라벨링 및 iOS 시스템 폼 요소가 적용된 고해상도 최종 시안 완성. |
| **가이드 탐색 (Explore)** | **초안** | `[Role] Senior Mobile App UI/UX Designer [Task] Design Explore screen for "FreshRoutine" [Design System] Modern iOS 18 HIG, White background, Teal point [Content] Huberman banner, template cards, Bottom Nav: [Today], [Explore], [Builder]...` | • 상단 배너 일러스트 및 카드 UI 구성은 우수하나 하단 탭 바 라벨이 영문(`Today`, `Explore`, `Builder`, `Report`, `My`)으로 생성됨. |
| | **수정** | `[Task] Revise Explore screen. Keep 1st-version layout exactly. Only change bottom tab labels to Korean. [Content] Tab labels: 오늘 / 탐색 / 만들기 / 리포트 / 마이 [Do Not Include] English tab labels...` | • 레이아웃 및 앤드류 휴버먼 배너를 유지하면서 하단 탭 바 라벨을 완전한 국문 5개 탭으로 변환 완료. |
| | **최종** | `Photorealistic iPhone app UI mockup. Clean card UI, Korean-only navigation bar, High fidelity Figma style.` | • 서비스 톤앤매너와 일치하는 탐색 라이브러리 및 통일된 탭 바 디자인 확정. |
| **구독 페이월 (PRO Paywall)** | **초안** | `[Role] Senior Mobile App UI/UX Designer [Task] Design Premium Paywall screen for "FreshRoutine PRO" [Design System] Soft Mint-to-White gradient, Dark Navy text, Gold/Teal accents [Content] Features, Plan cards: Annual Plan (BEST VALUE), Monthly Plan, 3-day trial CTA...` | • 플랜 카드 상단에 `BEST VALUE`, 하단에 영문 결제 안내 텍스트가 혼재되어 나타남. |
| | **수정** | `[Task] Revise PRO paywall screen. Keep layout exactly. Only replace leftover English with Korean. [Content] Annual badge: 최고 혜택, Prices: ₩3,900/월, ₩9,900/월, CTA: 3일 무료 체험 시작하기 [Do Not Include] BEST VALUE, billed annually...` | • 뱃지 텍스트를 `최고 혜택`으로 수정하고, 결제 금액 단위를 명확한 원화(`₩`) 및 국문 안내로 정돈. |
| | **최종** | `High-converting SaaS paywall design, clean typography, pure Korean copywriting, polished card layout.` | • 전환율 중심의 깔끔한 카드 레이아웃과 혜택 체크리스트를 갖춘 최종 페이월 완성. |

---

## 4. 프로토타입 구현 및 코드 변환 (Implementation)

* **Figma 인터랙션 & 핫스팟 구성**:
  * 하단 5개 탭 바(`오늘` / `탐색` / `만들기` / `리포트` / `마이`) 간의 화면 전환 네비게이션 연결
  * 루틴 목록 체크 토글 인터랙션 및 타이머 화면 오버레이 연결
  * 마이페이지 내 `FreshRoutine PRO` 배너 클릭 시 구독 결제 페이월 모달 오픈 인터랙션 구현
* **코드 변환 (React/V0)**:
  * 모바일 뷰포트(390px) 기준 반응형 프레임 컴포넌트 설계
  * React 기반 탭 전환 라우팅 및 폼 입력 상태 관리(`useState`) 구축
  * 테마 컬러(`Teal #1DB8A4`, `Slate #5B6E8A`, `Mint #D4F5EF`) 및 `Noto Sans KR` 폰트 시스템 반영

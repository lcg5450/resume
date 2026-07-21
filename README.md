# 이창귀

소프트웨어 엔지니어 · SDK 플랫폼 / iOS 개발자

- Email: lcg5450@gmail.com
- GitHub: https://github.com/lcg5450
- [상세 경력기술서](career_2026_ko.md)
- [이력서](resume_2026_ko.md)
- [기존 경력 기록](career_legacy_ko.md)

## 소개

2007년부터 현재까지 C/C++ 기반 미디어 소프트웨어, 모바일 단말, iOS 서비스, 플랫폼 SDK를 개발해 왔습니다. 대규모 방송 및 미디어 서비스의 앱 구조와 안정화를 담당했고, 현재는 여러 게임과 엔진이 공통으로 사용하는 SDK의 설계, 개발, 배포 자동화와 출시 지원을 수행하고 있습니다.

사용자에게 직접 전달되는 앱의 품질과 SDK를 사용하는 개발자의 통합 경험을 함께 이해하는 것이 강점입니다. 최근에는 모듈형 iOS 프레임워크, 네이티브-엔진 브리지, 결제 모듈, 음성 및 채팅, CI/CD와 멀티플랫폼 출시 문제 해결에 집중하고 있습니다.

## 대표 경험

### SDK 아키텍처 및 멀티플랫폼 연동

- Tuist 기반 Purpleworks SDK iOS 프레임워크 초기 설계 및 모듈형 구조 구축
- iOS 네이티브와 Unreal Engine 간 통신 브리지 구현
- 인증 WebView 호출을 iOS, Android, Windows 공통 인터페이스로 재설계
- 게임 연동 과정의 STL 문제를 해소하기 위해 C++ SDK를 C API 기반으로 전환하고 게임팀 제공 완료
- Unreal Engine, Unity, Cocos2d-x, CryEngine과 PS4, PS5, Nintendo Switch 환경 지원

### 빌드 및 배포 플랫폼

- Jenkins 내부의 빌드 스크립트를 Git으로 이관하고 SDK 및 샘플 앱의 빌드·배포 파이프라인 정비
- 동일 빌드의 프레임워크와 dSYM을 함께 보관해 산출물 추적 가능성 개선
- SDK 정기 배포 시간을 약 1시간에서 30분 내외로 단축
- Claude 스킬 기반 Jenkins Job Creator를 개발해 Job 생성 자동화

### 출시 및 품질 문제 해결

- Unreal Engine의 Swift 미지원 환경에서 Swift 런타임, 재서명 및 SwiftSupport 구성을 RemoteBuild 흐름에 자동화
- 실제 게임 프로젝트를 직접 빌드해 SDK 연동과 크래시를 재현하고 출시 문제 해결
- 아프리카TV iOS 앱 v2.0 아키텍처와 UI/UX 리뉴얼 주도
- 크래시 분석과 구조 개선으로 서비스 크래시율을 약 6%에서 1% 미만으로 개선

## 경력

| 회사 | 기간 | 역할 | 핵심 경험 |
| --- | --- | --- | --- |
| 엔씨소프트(NCSOFT) | 2018-현재 | SDK 플랫폼 / iOS 개발자 | SDK 설계, C API 전환, 엔진 연동, 결제, 음성 및 채팅, CI/CD, 출시 지원 |
| Azar | 2017.06-2018.06 | iOS 개발자 | Swift, RxSwift, WKWebView, WebRTC, GPUImage |
| 아프리카TV(현 SOOP) | 2012.10-2017.06 | iOS 애플리케이션 개발자 / 선임연구원 | 앱 아키텍처, 안정화, 라이브 플레이어, IAP, WebView |
| 인스모바일 | 2008.11-2012.09 | 모바일 소프트웨어 개발자 | PMP, 모바일 UI, 브라우저 포팅, Cocos2D iOS 게임 |
| 이전 경력 | 2007.05-2008.11 | 소프트웨어 개발자 | 멀티미디어 키오스크, DirectShow, MFC, 장비 I/O |

## 핵심 기술

- **언어:** Swift, Objective-C, C, C++, 셸 스크립트, Groovy
- **iOS / SDK:** iOS 프레임워크, XCFramework, SPM, Tuist, StoreKit2, WKWebView
- **게임 엔진 / 플랫폼:** Unreal Engine, Unity, Cocos2d-x, CryEngine, PS4, PS5, Nintendo Switch
- **미디어 / 실시간 통신:** WebRTC, Vivox, Google STT, TCP 음성채팅, ReplayKit, GPUImage
- **빌드 / 배포:** Jenkins, Git, Fastlane, CI/CD, Unreal Engine RemoteBuild
- **설계:** 모듈형 아키텍처, 공통 인터페이스, 네이티브-엔진 브리지, C API, SDK 패키징

세부 프로젝트, 역할과 성과는 [2026년 경력기술서](career_2026_ko.md)에서 확인할 수 있습니다.

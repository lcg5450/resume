# 이창귀

lcg5450@gmail.com

## 경력 요약

2007년부터 현재까지 C/C++ 기반 미디어 소프트웨어, 모바일 단말, iOS 서비스, 플랫폼 SDK를 개발해 온 소프트웨어 엔지니어입니다. 아프리카TV iOS 앱에서는 대규모 방송 및 미디어 서비스의 앱 구조, 라이브 플레이어, WebView 연동, 안정화 업무를 담당했고, 엔씨소프트에서는 여러 게임과 엔진이 공통으로 사용하는 SDK의 설계, 개발, 배포 자동화, 출시 지원을 수행했습니다.

최근 경력의 중심은 SDK를 하나의 제품처럼 설계하고 운영하는 일입니다. Tuist 기반 모듈형 iOS 프레임워크, Unreal 브리지, StoreKit2 결제 모듈, WKWebView 기반 인증 흐름, Jenkins 배포 파이프라인, dSYM 추적, 엔진, Xcode, 서명 이슈 대응을 경험했습니다. 최근에는 C++ SDK와 게임 사이의 STL 객체 메모리 소유권 문제로 발생한 런타임 크래시를 해결하기 위해 외부 인터페이스를 C API로 전환하고 게임팀 제공을 완료했습니다.

## 핵심 기술

- **iOS / SDK:** Swift, Objective-C, C, C++, iOS 프레임워크, XCFramework, SPM, Tuist, StoreKit2, WKWebView, 푸시, 로컬 알림
- **SDK 설계:** 모듈형 아키텍처, 공통 인터페이스, 네이티브-엔진 브리지, C API, SDK 패키징, 버전 관리, 샘플 앱
- **멀티플랫폼 연동:** Unreal Engine, Unity, Cocos2d-x, CryEngine, Unreal Engine RemoteBuild, iOS 서명, Xcode 호환성 대응
- **빌드 / 배포:** Jenkins, Groovy, 셸 스크립트, Git, Fastlane, CI/CD, 배포 이력 관리, 배포 자동화
- **미디어 / 음성:** 라이브 플레이어 연동, 동영상 플레이어 개발, WebRTC, Vivox, Google STT, TCP 음성채팅, ReplayKit, GPUImage
- **서비스 품질:** 크래시 분석, 앱 구조 개선, 네이티브-웹 연동, 커스텀 URL Scheme, 출시 문제 해결

## 경력

### 엔씨소프트(NCSOFT) | SDK 플랫폼 / iOS 개발자 | 2018-현재

- C++ SDK와 게임 사이의 STL 객체 메모리 소유권 문제로 발생한 런타임 크래시를 해결하기 위해 외부 인터페이스를 C API로 전환하고 게임팀 제공을 완료했습니다.
- Tuist 기반 Purpleworks SDK iOS 프레임워크와 Unreal Engine 통신 브리지를 초기 설계하고, 인증 WebView 호출을 iOS, Android, Windows 공통 인터페이스로 재설계해 세 플랫폼을 각각 담당하던 구조를 한 명이 일관되게 운영하고 유지보수할 수 있도록 단순화했습니다.
- StoreKit2 기반 IAP 모듈의 영수증, 주문, 아이템 배송 흐름을 표준화하고, Cocos2d-x 환경에 Purple Store 결제 및 반복 결제 UI를 제공해 내부 결제 전환과 수수료 절감 기반을 마련했습니다.
- Jenkins 내부의 빌드 스크립트를 Git으로 이관하고 SDK와 샘플 앱의 빌드 및 배포 파이프라인을 정비했으며, Claude 스킬 기반 Jenkins Job Creator로 Job 생성을 자동화했습니다.
- 동일 빌드의 프레임워크와 dSYM을 함께 보관해 산출물 추적 가능성을 높이고, SDK 정기 배포 시간을 약 1시간에서 30분 내외로 단축했습니다.
- Unreal Engine이 Swift를 공식 지원하지 않던 환경에서 Swift 런타임 라이브러리 포함 및 재서명과 SwiftSupport 디렉터리 구성을 RemoteBuild 흐름에 자동화해 Swift 기반 SDK의 iOS 출시 차단 문제를 해결했습니다.
- Unreal, Unity, Cocos2d-x, CryEngine과 PS4, PS5, Nintendo Switch 환경에서 SDK 연동, 빌드, 서명 및 음성채팅을 지원했습니다.
- 리니지2M 프로젝트를 직접 빌드해 SDK 연동과 크래시를 게임팀에 의존하지 않고 재현하고, 리니지2M, Battle Crush, Journey of Monarch, AION2, 호연, Lost Sword 등의 출시 문제를 지원했습니다.
- WebRTC, Vivox, Google STT, TCP 음성채팅 기반 음성 및 채팅 기능과 음성 녹음, 효과 및 번역 기능을 개발했습니다.

### Azar | iOS 개발자 | 2017.06-2018.06

- Swift와 RxSwift 기반으로 VIP, 프로필, 온보딩, 후면 카메라, 관심사 등 사용자 기능을 개발했습니다.
- WKWebView와 JavaScript 주입을 활용해 네이티브-웹 연동 기능을 구현했습니다.
- WebRTC, GPUImage 기반 미디어 기능 연동과 테스트 코드 개선을 수행했습니다.

### 아프리카TV(현 SOOP) | iOS 애플리케이션 개발자 / 선임연구원 | 2012.10-2017.06

- 국내 아프리카TV v2.0 아키텍처 설계와 UI/UX 전면 리뉴얼을 주도했습니다.
- 크래시 분석과 구조 개선으로 서비스 크래시율을 약 6%에서 1% 미만으로 개선했습니다.
- 라이브 플레이어를 연동하고 동영상 플레이어를 개발했으며, 팝업, 확대, 방송 필터 기능을 구현했습니다.
- IAP, 푸시, SNS, WKWebView 연동을 구현하고 약 70개 커스텀 URL Scheme를 처리하는 공통 모듈을 개발했습니다.
- 일본 아프리카TV 개발, 글로벌 앱 리팩토링, CocoaPods 기반 라이브러리 관리 체계 구축에 참여했습니다.

### 인스모바일 | 모바일 소프트웨어 개발자 | 2008.11-2012.09

- Samsung Yepp R2 등 PMP의 사진 및 텍스트 뷰어와 동영상 플레이어 UI를 개발했습니다.
- SCH-U365 모바일 브라우저를 포팅하고 버그를 수정했으며, Cocos2D 기반 iOS 게임을 개발했습니다.

### 이전 경력 | 소프트웨어 개발자 | 2007.05-2008.11

- 멀티미디어 키오스크 시스템의 GUI, DirectShow 기반 영상 인코딩 및 디코딩, MMS 전송용 인코딩 프로그램, 장비 I/O 제어 프로그램을 개발했습니다.

# 이창귀 경력기술서

lcg5450@gmail.com

## 경력 요약

2007년부터 현재까지 C/C++ 기반 미디어 소프트웨어, 모바일 단말, iOS 서비스, 플랫폼 SDK를 개발했습니다. 초기에는 DirectShow, MFC, PMP 및 모바일 단말 소프트웨어를 개발했고, 이후 아프리카TV iOS 앱에서 방송 및 미디어 서비스의 앱 구조, 라이브 플레이어, 결제, WebView, 안정화 업무를 담당했습니다. 엔씨소프트에서는 여러 게임과 엔진에서 공통으로 사용하는 SDK의 iOS 프레임워크, 네이티브-엔진 브리지, 결제 모듈, 음성 및 채팅, CI/CD, 출시 지원을 수행했습니다.

경력의 강점은 사용자에게 직접 전달되는 앱 품질과 SDK를 사용하는 개발자의 통합 경험을 모두 이해한다는 점입니다. 대규모 iOS 서비스에서는 크래시율 개선과 UI/UX 개편을 주도했고, 플랫폼 SDK 영역에서는 모듈형 아키텍처, 공통 인터페이스, 빌드 및 배포 자동화, 샘플 앱, dSYM 추적, 엔진, Xcode, 서명 이슈 대응을 통해 SDK 운영 품질을 개선했습니다.

## 대표 경험

### 지속적으로 개선한 SDK 배포 플랫폼

SDK 배포 자동화를 일회성 작업이 아닌 게임팀과 SDK 개발자가 계속 사용하는 내부 플랫폼으로 바라보고 개선했습니다. Jenkins 내부에 분산된 빌드 스크립트를 Git으로 이관하고 네이티브 SDK, 엔진 SDK, 샘플 앱의 빌드와 배포 흐름을 연결했습니다. 배포 이력과 산출물을 추적할 수 있는 구조를 마련하고 운영 방법을 문서화해 특정 담당자에게 집중된 업무를 팀이 함께 운영할 수 있도록 확장했습니다.

그 결과 SDK 정기 배포 시간을 약 1시간에서 30분 내외로 단축했습니다. 최근에는 Claude 스킬 기반 Jenkins Job Creator를 개발해 Job 생성을 자동화했습니다. 실제 사용 과정에서 발견한 불편을 계속 해소해 왔습니다.

### Unreal Engine의 Swift 미지원 환경에서 리니지2M 출시 문제 해결

리니지2M 출시 당시 Unreal Engine의 자동화 도구는 Swift를 공식 지원하지 않았고, Swift 기반 CommunitySDK를 포함한 앱을 기존 방식으로 App Store에 업로드할 수 없었습니다. Xcode와 IPA 산출물 구조를 분석한 뒤 Swift 런타임 라이브러리를 앱에 포함하고 재서명했으며, App Store 검증에 필요한 SwiftSupport 디렉터리를 구성하는 과정을 자동화했습니다. 이를 Unreal Engine의 RemoteBuild 흐름에 적용해 Swift 기반 SDK의 iOS 출시 차단 문제를 해결했습니다.

이와 별도로 게임팀에 재현을 요청하는 데 그치지 않고 리니지2M 프로젝트 소스를 직접 내려받아 로컬 빌드 환경을 구성했습니다. SDK 연동 방식과 크래시를 독립적으로 재현하고 수정 사항을 실제 게임 프로젝트에서 검증해 게임팀에 의존하지 않는 문제 해결 체계를 마련했습니다.

### 아프리카TV 사용자 경험과 안정성 개선

국내 아프리카TV iOS 앱을 운영하며 기능 추가뿐 아니라 사용자가 체감하는 안정성과 시청 경험을 개선하는 데 집중했습니다. 크래시를 분석하고 앱 구조를 개선해 서비스 크래시율을 약 6%에서 1% 미만으로 낮췄으며, v2.0 아키텍처 설계와 UI/UX 전면 리뉴얼을 주도했습니다.

라이브 플레이어 연동과 동영상 플레이어 개발, 팝업 및 확대 기능, 방송 필터를 적용해 시청 경험을 개선했습니다. 또한 약 70개 커스텀 URL Scheme를 공통 모듈로 통합해 여러 서비스 진입 경로를 일관되게 처리할 수 있도록 했습니다.

## 핵심 역량

### iOS SDK 설계

- Tuist 기반 모듈형 iOS 프레임워크 초기 설계 및 모듈 경계 수립
- Objective-C, Swift, C, C++ 기반 네이티브 SDK 개발
- XCFramework 및 Swift Package Manager 지원
- 인증 WebView, StoreKit2 IAP, 사용자 프로필, 로컬 푸시 기능 개발
- STL 객체의 메모리 소유권 문제로 발생한 런타임 크래시 해결 및 C++ SDK의 C API 전환
- SDK 기능 추가와 교체, 장기 유지보수를 고려한 프로젝트 구조 설계

### 멀티플랫폼 SDK 연동

- Unreal Engine, Unity, Cocos2d-x, CryEngine용 SDK 플러그인 및 샘플 앱 개발과 지원
- iOS 네이티브와 Unreal Engine 간 통신 브리지 구현
- Unreal Engine의 RemoteBuild, Swift 런타임, iOS 서명, Xcode 버전 변화 대응
- PS4, PS5, Nintendo Switch 등 콘솔 플랫폼 관련 빌드 및 음성채팅 환경 지원
- 실제 게임 프로젝트 소스를 빌드해 SDK 연동 문제와 크래시를 재현하고 해결

### 빌드 및 배포 체계

- Jenkins, Groovy, 셸 스크립트, Git 기반 CI/CD 파이프라인 설계 및 운영
- SDK, 엔진 SDK, 샘플 앱 빌드와 배포 서버 업로드 자동화
- 동일 빌드 프레임워크와 dSYM 보관 구조 개선
- 배포 이력, 테스트 정보, 산출물 추적 가능성 개선
- 수작업 릴리스 단계와 특정 담당자 의존도 축소

### iOS 서비스 및 제품 품질

- 아프리카TV iOS 앱 v2.0 아키텍처 설계와 UI/UX 리뉴얼
- 라이브 플레이어 연동 및 동영상 플레이어 개발
- IAP, 푸시 알림, SNS, WKWebView, 커스텀 URL Scheme 연동
- 크래시 분석과 앱 구조 개선을 통한 안정화
- 국내, 일본, 글로벌 방송 및 미디어 앱 개발과 운영 경험

### 실시간 미디어 및 음성

- WebRTC, Vivox, Google STT, TCP 음성채팅 연동
- 음성 필터, 녹음, 효과, 번역 기능 개발
- Purple Live, Purple Voice, Nintendo Switch 음성채팅 지원
- WebRTC 버전 업데이트, XCFramework, Apple Silicon, 엔진 제약 대응

## 경력 개요

| 회사 | 기간 | 역할 | 핵심 경험 |
| --- | --- | --- | --- |
| 엔씨소프트(NCSOFT) | 2018-현재 | SDK 플랫폼 / iOS 개발자 | SDK 설계, C API 전환, 엔진 연동, 결제, 음성 및 채팅, CI/CD, 출시 지원 |
| Azar | 2017.06-2018.06 | iOS 개발자 | Swift 및 RxSwift 기능 개발, WKWebView 네이티브-웹 연동, WebRTC, GPUImage |
| 아프리카TV(현 SOOP) | 2012.10-2017.06 | iOS 애플리케이션 개발자 / 선임연구원 | 대규모 iOS 서비스, 앱 안정화, 라이브 플레이어, IAP, WebView |
| 인스모바일 | 2008.11-2012.09 | 모바일 소프트웨어 개발자 | PMP, 모바일 UI, 브라우저 포팅, Cocos2D iOS 게임 |
| 이전 경력 | 2007.05-2008.11 | 소프트웨어 개발자 | 멀티미디어 키오스크, DirectShow, MFC, 장비 I/O |

## 상세 경력

### 엔씨소프트(NCSOFT) | SDK 플랫폼 / iOS 개발자 | 2018-현재

iOS 네이티브 프레임워크, 게임 엔진 플러그인, 음성 및 채팅 SDK, 빌드 및 배포 자동화, 출시 지원까지 플랫폼 SDK의 전체 개발 및 운영 과정을 담당했습니다. 2018년 MediaSDK 및 UI 개발로 시작해 CommunitySDK 통합과 멀티 엔진 지원을 거쳤고, 2025년에는 Purpleworks SDK의 신규 아키텍처와 주요 제품 기능을 초기 설계부터 주도했습니다. 최근에는 C++ SDK와 게임 사이의 STL 객체 메모리 소유권 문제로 발생한 런타임 크래시를 해결하기 위해 외부 인터페이스를 C API로 전환하고 게임팀 제공을 완료했습니다.

#### C++ SDK의 C API 전환 | 2026

**주요 역할**

- C++ SDK와 게임 사이에서 발생한 STL 객체 메모리 소유권 문제와 런타임 크래시 분석
- SDK 경계의 메모리 소유권을 명확히 관리할 수 있도록 외부 인터페이스를 C API 기반으로 재설계
- 기존 C++ SDK 기능을 C API 방식으로 전환하고 게임팀 적용 지원

**성과**

- STL 객체의 메모리 소유권 문제로 발생한 런타임 크래시 해결
- 게임팀에서 적용 가능한 C API 기반 SDK 전환과 제공 완료

#### Purpleworks SDK 설계 및 제품 기능 신규 개발 | 2025

**주요 역할**

- Tuist 기반 Purpleworks SDK iOS 프레임워크를 초기 설계부터 구축
- 기능별 책임을 분리한 모듈형 구조 설계
- iOS 네이티브와 Unreal Engine 간 통신 브리지 구현
- 인증 WebView 호출 흐름을 iOS, Android, Windows 공통 인터페이스로 재설계
- StoreKit2 기반 IAP 모듈 재구성
- 결제 영수증, 주문, 아이템 배송 프로세스 표준화
- 사용자 프로필 조회 구조 통합 및 이벤트와 복귀 알림용 로컬 푸시 개발
- Purpleworks SDK와 기존 NC Platform 및 CommunitySDK 병행 유지보수

**성과**

- 신규 SDK의 iOS 개발 기반과 장기 유지보수를 위한 아키텍처 기준 수립
- 인증 WebView 호출을 iOS, Android, Windows 공통 인터페이스로 재설계해, 기존에 세 플랫폼을 각각 담당하던 구조를 한 명이 일관되게 운영하고 유지보수할 수 있도록 단순화
- 결제 성공 후 아이템 미배송 유형을 줄이기 위한 설계 구조와 복원 기반 예외 처리 경로 마련
- 리니지2M, 호연, Lost Sword, AION2 출시 과정의 플랫폼 및 빌드 이슈 병행 지원
- Cocos 엔진에 Purple Store 결제 및 반복 결제 UI를 제공해 외부 결제 의존도를 낮추고 수수료를 절감할 수 있는 내부 결제 전환 기반 마련

#### CI/CD 및 배포 체계 고도화 | 2019-현재

**주요 역할**

- CommunitySDK 빌드와 게임 엔진 샘플 앱 적용, 배포 서버 업로드를 Jenkins Pipeline으로 연결
- Jenkins 내부에 분산된 빌드 스크립트를 Git 저장소로 이관
- iOS 네이티브, Unreal, 플랫폼별 샘플 앱 파이프라인 구현
- 네이티브와 게임 엔진의 분리된 파이프라인을 연결해 동일 빌드 프레임워크와 dSYM 보관
- 5대 빌드 서버의 산출물을 Git으로 관리해 서버별 접속 없이 결과와 배포 이력을 확인할 수 있는 구조 구축
- Unreal 4.25, 4.27, 5.0.3 및 PS4, PS5, Switch 조합을 확장할 수 있도록 Declarative Pipeline 개선
- 브랜치, 플랫폼, 엔진 옵션을 선택할 수 있는 Manual Pipeline 제공
- SDK 버전, 테스트 정보, 품질 단계가 배포 시점에 남도록 프로덕트기술서 산출 자동화
- Claude 스킬 기반 Jenkins Job Creator를 개발해 Job 생성 자동화

**성과**

- SDK 정기 배포 시간을 약 1시간에서 30분 내외로 단축
- 수작업 배포와 dSYM 불일치 가능성을 줄이고 릴리스 재현성과 추적 가능성 향상
- 특정 담당자에게 집중된 Jenkins 업무를 문서화하고 공유해 팀 내 추가 운영 인력 확보
- 빌드 스크립트 형상 관리로 변경 이력과 책임 범위를 명확히 함

#### 게임 엔진 연동 및 출시 문제 해결 | 2019-2025

**주요 역할**

- Unreal의 Swift 공식 지원이 부족한 환경에서 Swift 런타임 라이브러리 포함 및 재서명, SwiftSupport 디렉터리 구성과 RemoteBuild 자동화 구현
- 리니지2M 프로젝트 소스를 직접 내려받아 로컬 빌드하고 SDK 연동과 크래시를 게임팀에 의존하지 않고 재현
- Cocos2d-x 샘플 앱에 채팅 및 음성채팅 기능 추가
- Unreal 샘플 앱의 Blueprint 로직을 C++ 코드로 재작성
- Unreal, Unity, Cocos2d-x, CryEngine 연동과 Xcode, macOS, Swift Standard Library 변화에 따른 빌드 문제 대응
- Journey of Monarch의 Unreal Engine 5.4, RemoteBuild 및 서명 이슈 지원
- Battle Crush의 iOS Audio Session, 블레이드엔소울2의 Swift 라이브러리 누락 문제 해결
- Xcode 12-15, Unity 2022, Apple Silicon, SPM 등 플랫폼 요구사항 대응

**성과**

- Swift 기반 SDK의 Unreal Engine 기반 iOS 출시 차단 위험을 해소하고 실제 게임 프로젝트에서 검증 가능한 지원 체계 구축
- Swift 런타임 누락, 서명 명령 변경 등 출시 단계의 환경 의존 문제 해결
- 반복적으로 발생한 연동 문제를 SDK, 스크립트, 샘플 앱 개선에 반영

**주요 지원 프로젝트**
리니지2M, Battle Crush, Journey of Monarch, AION2, 호연, Lost Sword, PuzzleUp, LineageW, 블레이드엔소울2

#### 음성, 채팅 및 실시간 미디어 플랫폼 | 2020-2024

**주요 역할**

- iOS Voice Input에서 Audio Filter를 거쳐 WebRTC Layer로 전달되는 오디오 경로 수정
- Purple Live용 CommunityLive SDK의 음성 필터 및 사용자 지정 모드 지원
- Unreal 음성 녹음과 Google STT 모듈을 추가해 게임 내 음성 번역 기능 지원
- 음성 녹음 및 효과 재생 기능을 개발해 Purple App에 제공
- Vivox 기반 Nintendo Switch 음성채팅 API와 WebRTC 미지원 환경용 TCP 음성채팅 개발
- WebRTC M93, M106, M124 버전 빌드 및 적용, XCFramework와 Apple Silicon 대응

**성과**

- Purple Live와 Purple Voice, 게임 음성 번역, 음성 효과 등 실시간 음성 기능을 SDK로 제공
- WebRTC를 사용할 수 없는 Switch 환경까지 음성채팅 지원 범위 확장
- 게임 엔진 및 Apple Silicon 환경의 배포 제약에 맞춰 XCFramework와 프레임워크 변환 경로 제공

### Azar | iOS 개발자 | 2017.06-2018.06

Swift와 RxSwift 기반으로 iOS 앱의 사용자 기능과 네이티브-웹 연동 기능을 개발했습니다.

**주요 역할**

- VIP, 프로필, 온보딩, 후면 카메라, 관심사 기능 개발
- WKWebView 기반 네이티브-웹 연동
- JavaScript 주입을 활용한 WebView 기능 확장
- RxSwift 기반 이벤트 처리
- 테스트 케이스 작성 및 테스트 커버리지 개선
- WebRTC, GPUImage 기반 미디어 기능 연동

### 아프리카TV(현 SOOP) | iOS 애플리케이션 개발자 / 선임연구원 | 2012.10-2017.06

국내 및 일본 아프리카TV iOS 애플리케이션을 개발하고 운영하며 앱 아키텍처, UI/UX, 라이브 플레이어 연동, 동영상 플레이어 개발, 결제, 푸시, WebView 연동과 서비스 안정화를 담당했습니다.

**주요 역할**

- 국내 아프리카TV iOS 앱 신규 기능 개발 및 유지보수
- 아프리카TV v2.0 아키텍처 설계와 UI/UX 전면 리뉴얼
- 라이브 플레이어 연동 및 동영상 플레이어 개발
- App Store IAP, 푸시 알림, SNS 로그인 및 공유 기능 구현
- UIWebView에서 WKWebView로 전환
- 약 70개 커스텀 URL Scheme를 처리하는 공통 모듈 개발
- 일본 아프리카TV 앱 개발 및 글로벌 앱 리팩토링 참여
- CocoaPods와 Git Submodule 기반 라이브러리 모듈화 및 iOS 버전 변화 대응

**성과**

- 크래시 분석과 앱 구조 개선으로 서비스 크래시율을 약 6%에서 1% 미만으로 개선
- 국내 아프리카TV v2.0의 구조 설계와 UI/UX 리뉴얼 주도
- 라이브 플레이어 팝업 및 확대 기능과 GPUImage 기반 방송 필터 적용
- WebView와 네이티브 연동을 공통화해 다수의 서비스 진입 경로를 일관되게 처리
- 국내 서비스 운영 경험을 일본과 글로벌 프로젝트로 확장

### 인스모바일 | 모바일 소프트웨어 개발자 | 2008.11-2012.09

스마트폰과 PMP 플랫폼을 대상으로 시스템 UI, 미디어 애플리케이션, 모바일 브라우저와 iOS 게임을 개발했습니다.

**주요 역할**

- Samsung Yepp R2 등 PMP의 사진 및 텍스트 뷰어와 동영상 플레이어 UI 개발
- SCH-U365 모바일 브라우저 포팅 및 버그 수정
- Cocos2D 기반 Jumping Race iOS 게임 개발
- R2 모바일 애플리케이션 및 교육용 콘텐츠 애플리케이션 개발

**주요 프로젝트**
Samsung Yepp R2, MarvelQ, SCH-U365 Browser Porting, Jumping Race(iOS), R2 모바일 애플리케이션, 교육용 콘텐츠 애플리케이션

### 이전 경력 - 동영상 키오스크 개발 | 소프트웨어 개발자 | 2007.05-2008.11

멀티미디어 키오스크 시스템의 GUI와 영상 처리 기능을 구현했습니다.

- 동영상 촬영 키오스크 GUI 개발
- DirectShow 기반 영상 인코딩 및 디코딩 기능 개발
- MMS 전송용 인코딩 프로그램 개발
- 장비 I/O 제어 프로그램 개발

## 기술

- **언어:** Swift, Objective-C, C, C++, 셸 스크립트, Groovy
- **Apple 플랫폼:** iOS 프레임워크, XCFramework, SPM, Tuist, StoreKit, StoreKit2, WKWebView, 푸시, 로컬 알림, Apple Silicon
- **게임 엔진 / 플랫폼:** Unreal Engine, Unity, Cocos2d-x, CryEngine, PS4, PS5, Nintendo Switch
- **미디어 / 실시간 통신:** 라이브 플레이어 연동, 동영상 플레이어 개발, WebRTC, Vivox, Google STT, TCP 음성채팅, ReplayKit
- **빌드 / 배포:** Jenkins, Git, Fastlane, CI/CD, Unreal Engine RemoteBuild, 버전 관리, 배포 자동화
- **설계:** 모듈형 아키텍처, 공통 인터페이스, 네이티브-엔진 브리지, C API, SDK 패키징

## 경력 발전 과정

C/C++ 기반 미디어 및 단말 소프트웨어 개발로 시작해 대규모 iOS 서비스의 구조와 안정화를 담당했고, 이후 멀티 엔진 SDK 연동과 배포 자동화, 음성 및 채팅 플랫폼, 신규 SDK 아키텍처 설계로 역할을 확장했습니다. 기능 개발자에서 서비스 품질을 책임지는 iOS 엔지니어를 거쳐, 여러 제품과 개발팀이 공통으로 사용하는 플랫폼의 구조와 운영 체계를 설계하는 SDK 플랫폼 엔지니어로 성장해 왔습니다.

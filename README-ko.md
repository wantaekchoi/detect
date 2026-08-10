![License: Unlicense](https://img.shields.io/github/license/wantaekchoi/detect)

[English](README.md) | [한국어](README-ko.md)

# Detect

브라우저 및 장치 기능 감지 페이지

**라이브 데모**: https://wantaekchoi.github.io/detect/

- [MDN: Feature Detection Guide](https://developer.mozilla.org/docs/Learn_web_development/Extensions/Testing/Feature_detection)
- [MDN: 사용자 에이전트를 사용한 브라우저 감지](https://developer.mozilla.org/ko/docs/Web/HTTP/Guides/Browser_detection_using_the_user_agent)

## 동작 방식

각 체크는 `{ expr, fn }` 쌍으로 정의되고 공용 `try/catch` 안에서 실행됩니다. 현재 브라우저에 해당 API가 없으면(예: `ServiceWorkerRegistration`을 지원 안 하는 구형 브라우저) 그 체크는 페이지를 죽이지 않고 그냥 `false`로 표시됩니다 — API 하나가 없다고 나머지 결과까지 전부 날아가지 않습니다.

## 주요 기능
- **navigator.userAgent**: [브라우저 및 OS 정보](https://developer.mozilla.org/docs/Web/API/Navigator/userAgent)
- **navigator.language**: [브라우저 선호 언어](https://developer.mozilla.org/docs/Web/API/Navigator/language)
- **screen.width, screen.height**: [화면 해상도](https://developer.mozilla.org/docs/Web/API/Screen)
- **navigator.maxTouchPoints**: [터치 지원 여부](https://developer.mozilla.org/docs/Web/API/Navigator/maxTouchPoints)
- **navigator.hardwareConcurrency**: [논리 CPU 코어 수](https://developer.mozilla.org/docs/Web/API/Navigator/hardwareConcurrency)
- **'serviceWorker' in navigator**: [서비스워커 지원 (오프라인 캐싱)](https://developer.mozilla.org/docs/Web/API/Service_Worker_API)
- **'localStorage' in window**: [로컬 스토리지 지원](https://developer.mozilla.org/docs/Web/API/Window/localStorage)
- **'geolocation' in navigator**: [위치 정보 API 지원](https://developer.mozilla.org/docs/Web/API/Geolocation_API)
- **typeof matchMedia === 'function'**: [미디어 쿼리 API 지원](https://developer.mozilla.org/docs/Web/API/Window/matchMedia)
- **matchMedia('(prefers-color-scheme: dark)').matches**: [다크 모드 선호 감지](https://developer.mozilla.org/docs/Web/CSS/@media/prefers-color-scheme)
- **'indexedDB' in window**: [IndexedDB 지원](https://developer.mozilla.org/docs/Web/API/IndexedDB_API)
- **'WebSocket' in window**: [WebSocket 지원](https://developer.mozilla.org/docs/Web/API/WebSocket)
- **'RTCPeerConnection' in window**: [WebRTC 지원](https://developer.mozilla.org/docs/Web/API/RTCPeerConnection)
- **navigator.onLine**: [온라인/오프라인 상태](https://developer.mozilla.org/docs/Web/API/Navigator/onLine)
- **'connection' in navigator && navigator.connection.effectiveType**: [체감 네트워크 등급 (Network Information API)](https://developer.mozilla.org/docs/Web/API/NetworkInformation/effectiveType)
- **CSS.supports('display','grid')**: [CSS Grid 지원](https://developer.mozilla.org/docs/Web/API/CSS/supports)
- **'WebAssembly' in window**: [WebAssembly 지원](https://developer.mozilla.org/docs/WebAssembly)
- **'WebGLRenderingContext' in window**: [WebGL 지원](https://developer.mozilla.org/docs/Web/API/WebGLRenderingContext)
- **'ontouchstart' in window**: [터치 이벤트 지원](https://developer.mozilla.org/docs/Web/API/GlobalEventHandlers/ontouchstart)
- **'PointerEvent' in window**: [포인터 이벤트 지원](https://developer.mozilla.org/docs/Web/API/PointerEvent)
- **'pointerEnabled' in Navigator.prototype**: [포인터 기기 유형 감지](https://developer.mozilla.org/docs/Web/API/Navigator/pointerEnabled)
- **'DeviceOrientationEvent' in window**: [디바이스 방향 이벤트 지원](https://developer.mozilla.org/docs/Web/API/DeviceOrientationEvent)
- **'PushManager' in window**: [Push API 지원](https://developer.mozilla.org/docs/Web/API/PushManager)
- **'Notification' in window**: [Notification API 지원](https://developer.mozilla.org/docs/Web/API/Notification)
- **'PaymentRequest' in window**: [Payment Request API 지원](https://developer.mozilla.org/docs/Web/API/Payment_Request_API)
- **'clipboard' in navigator**: [클립보드 API 지원](https://developer.mozilla.org/docs/Web/API/Clipboard_API)
- **'share' in navigator**: [웹 공유 API 지원](https://developer.mozilla.org/docs/Web/API/Navigator/share)
- **typeof navigator.getInstalledRelatedApps === 'function'**: [설치된 관련 앱 API 지원](https://developer.mozilla.org/docs/Web/API/Navigator/getInstalledRelatedApps)
- **typeof navigator.getBattery === 'function'**: [배터리 상태 API 지원](https://developer.mozilla.org/docs/Web/API/Battery_Status_API)
- **'mediaDevices' in navigator && 'getUserMedia' in navigator.mediaDevices**: [카메라·마이크 접근](https://developer.mozilla.org/docs/Web/API/MediaDevices)
- **'sync' in ServiceWorkerRegistration.prototype**: [백그라운드 동기화 지원](https://developer.mozilla.org/docs/Web/API/Background_Synchronization_API)

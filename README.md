[English](README.md) | [한국어](README-ko.md)

# Detect

A simple browser and device feature detection.

## Features
- **navigator.userAgent**: Browser and OS information ([MDN](https://developer.mozilla.org/docs/Web/API/Navigator/userAgent))
- **screen.width, screen.height**: Screen resolution ([MDN](https://developer.mozilla.org/docs/Web/API/Screen))
- **navigator.maxTouchPoints**: Touch support ([MDN](https://developer.mozilla.org/docs/Web/API/Navigator/maxTouchPoints))
- **'serviceWorker' in navigator**: Service Worker support (offline caching) ([MDN](https://developer.mozilla.org/docs/Web/API/Service_Worker_API))
- **'localStorage' in window**: LocalStorage support (client-side storage) ([MDN](https://developer.mozilla.org/docs/Web/API/Window/localStorage))
- **'geolocation' in navigator**: Geolocation API support ([MDN](https://developer.mozilla.org/docs/Web/API/Geolocation_API))
- **typeof matchMedia === 'function'**: Media Queries API support ([MDN](https://developer.mozilla.org/docs/Web/API/Window/matchMedia))
- **matchMedia('(prefers-color-scheme: dark)').matches**: Dark-mode preference detection ([MDN](https://developer.mozilla.org/docs/Web/CSS/@media/prefers-color-scheme))
- **'indexedDB' in window**: IndexedDB support (client database) ([MDN](https://developer.mozilla.org/docs/Web/API/IndexedDB_API))
- **'WebSocket' in window**: WebSocket support (real-time messaging) ([MDN](https://developer.mozilla.org/docs/Web/API/WebSocket))
- **'RTCPeerConnection' in window**: WebRTC support (real-time media) ([MDN](https://developer.mozilla.org/docs/Web/API/RTCPeerConnection))
- **CSS.supports('display','grid')**: CSS Grid support ([MDN](https://developer.mozilla.org/docs/Web/API/CSS/supports))
- **'WebAssembly' in window**: WebAssembly support (high-performance modules) ([MDN](https://developer.mozilla.org/docs/WebAssembly))
- **'WebGLRenderingContext' in window**: WebGL support (3D graphics) ([MDN](https://developer.mozilla.org/docs/Web/API/WebGLRenderingContext))
- **'ontouchstart' in window**: Touch event support ([MDN](https://developer.mozilla.org/docs/Web/API/GlobalEventHandlers/ontouchstart))
- **'PointerEvent' in window**: Pointer event support ([MDN](https://developer.mozilla.org/docs/Web/API/PointerEvent))
- **'pointerEnabled' in Navigator.prototype**: Pointer device type detection ([MDN](https://developer.mozilla.org/docs/Web/API/Navigator/pointerEnabled))
- **'DeviceOrientationEvent' in window**: Device orientation event support ([MDN](https://developer.mozilla.org/docs/Web/API/DeviceOrientationEvent))
- **'PushManager' in window**: Push API support (background push) ([MDN](https://developer.mozilla.org/docs/Web/API/PushManager))
- **'Notification' in window**: Notification API support ([MDN](https://developer.mozilla.org/docs/Web/API/Notification))
- **'PaymentRequest' in window**: Payment Request API support (one-click checkout) ([MDN](https://developer.mozilla.org/docs/Web/API/Payment_Request_API))
- **typeof navigator.getInstalledRelatedApps === 'function'**: Installed Related Apps API (deep-link branching) ([MDN](https://developer.mozilla.org/docs/Web/API/Navigator/getInstalledRelatedApps))
- **typeof navigator.getBattery === 'function'**: Battery Status API support ([MDN](https://developer.mozilla.org/docs/Web/API/Battery_Status_API))
- **'mediaDevices' in navigator && 'getUserMedia' in navigator.mediaDevices**: Camera & microphone access ([MDN](https://developer.mozilla.org/docs/Web/API/MediaDevices))
- **'sync' in ServiceWorkerRegistration.prototype**: Background Sync support ([MDN](https://developer.mozilla.org/docs/Web/API/Background_Synchronization_API))

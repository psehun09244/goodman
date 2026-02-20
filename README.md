# 사육관리표 Android 앱 빌드 가이드

## 📁 프로젝트 구조
이 폴더가 완성된 Android Studio 프로젝트입니다.

## 🛠️ 빌드 방법 (무료, 5분)

### 방법 1: Android Studio (권장)
1. **Android Studio 설치**: https://developer.android.com/studio
2. **프로젝트 열기**: File → Open → 이 폴더(SaeyukApp) 선택
3. **빌드**: Build → Build Bundle(s)/APK(s) → Build APK(s)
4. APK 파일 생성됨: `app/build/outputs/apk/debug/app-debug.apk`
5. 휴대폰에 APK 복사 후 설치 (설정 → 알 수 없는 소스 허용 필요)

### 방법 2: 온라인 빌드 (Android Studio 없이)
1. 이 프로젝트 폴더를 GitHub에 업로드
2. https://appetize.io 또는 https://buildozer.io 사용

## 📱 앱 특징
- **네이티브 Android 앱** (WebView 기반)
- **실제 휴대폰 알림** (시스템 알림 트레이)
- **localStorage 데이터 영구 저장**
- **오프라인 동작**
- **홈 화면 아이콘** (일반 앱처럼)

## 🔔 알림 작동 방식
HTML 앱에서 `AndroidBridge.scheduleNotification(title, body, delayMs, tag)` 호출 시
→ Android 시스템 알림 트레이에 실제 알림 표시

## ⚠️ 설치 전 확인
- 설정 → 보안 → "알 수 없는 출처" 허용
- 앱 설치 후 알림 권한 허용

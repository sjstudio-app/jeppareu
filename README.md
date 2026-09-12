# 제빠르 (Jeppareu)

빠르고 가벼운 macOS 네이티브 키보드 검색·실행 런처.

Jeppareu(제빠르)는 반응성이 중요한 핵심 작업 흐름을 네이티브 macOS 환경에서 지연 없이 수행할 수 있도록 설계된 생산성 도구입니다.

---

## 📌 저장소 안내 (Repository Notice)

본 저장소(`sjstudio-app/jeppareu`)는 제빠르(Jeppareu)의 **공식 공개 배포(Releases) 및 사용자 기술 지원(Issues)**을 위한 창구입니다.

- **소프트웨어 라이선스 정책**: 제빠르는 SJ Studio가 개발한 **무료 독점 소프트웨어(Free Proprietary Software)**입니다. 오픈소스 라이선스(MIT, Apache, GPL 등)로 배포되지 않으며, **소스 코드는 비공개(Private)로 안전하게 관리**됩니다.
- **배포 창구**: 공식 빌드 패키지(`.zip`) 및 체크섬은 [GitHub Releases](https://github.com/sjstudio-app/jeppareu/releases)를 통해서만 공개 배포됩니다.
- **지원 및 피드백**: 버그 제보, 사용 문의, 기능 제안은 [GitHub Issues](https://github.com/sjstudio-app/jeppareu/issues)를 이용해 주시기 바랍니다.

---

## 🚀 주요 기능 (Core Features)

- **전역 단축키 런처 (`⌥Space`)**: 마우스 없이 즉각적인 런처 호출 및 텍스트 포커스 획득
- **세 가지 검색 모드 순환 (`⌘[`, `⌘]`)**: All (통합) ⇄ Clipboard (클립보드) ⇄ Files (파일 시스템)
- **로컬 클립보드 히스토리**: 로컬 SQLite WAL 기반 영구 저장, 메모리 스냅샷 기반 초고속 검색, 자동 붙여넣기 (`Return`)
- **파일 시스템 직접 경로 및 통합 검색**: 절대 경로(`/`) 및 홈 경로(`~`) 즉시 검증 고정, Spotlight 비동기 인덱스 실시간 검색, 앱 실행 및 Finder 열기
- **Local-First & Zero-Network**: 외부 통신, 클라우드 동기화, 사용자 분석 텔레메트리(SDK) 일체 배제

---

## 📥 다운로드 및 설치 (Download & Installation)

1. [GitHub Releases](https://github.com/sjstudio-app/jeppareu/releases)에서 최신 버전의 `Jeppareu-<VERSION>.zip`을 다운로드합니다.
2. 압축을 풀고 `Jeppareu.app`을 `/Applications` (응용 프로그램) 폴더로 이동합니다.
3. 앱을 실행하고 화면의 안내에 따라 **손쉬운 사용 (Accessibility)** 권한을 허용합니다. (런처 항목 선택 시 직전 작업 앱으로 자동 붙여넣기를 실행하는 데 필요합니다.)
4. `⌥Space`를 눌러 런처를 실행합니다.

> **시스템 요구사항**:
> - Apple Silicon Mac (M1 / M2 / M3 / M4)
> - macOS 14.0 (Sonoma) 이상
> - Apple Developer ID 정식 코드 서명 및 Apple Notarization(공증) 완료

---

## 📖 문서 및 정책 (Documentation & Policies)

- [사용자 가이드 및 지원 안내 (SUPPORT.md)](SUPPORT.md)
- [개인정보 처리방침 (PRIVACY.md)](PRIVACY.md)
- [최종 사용자 사용권 계약 (EULA.md)](EULA.md)

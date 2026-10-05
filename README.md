# 제빠르 (Jeppareu)

빠르고 가벼운 macOS 네이티브 키보드 검색·실행 런처.

🌐 소개 페이지: [sjstudio.app/jeppareu](https://sjstudio.app/jeppareu)

Jeppareu(제빠르)는 반응성이 중요한 핵심 작업 흐름을 네이티브 macOS 환경에서 지연 없이 수행할 수 있도록 설계된 생산성 도구입니다.
상주 백그라운드 프로세스로 동작하여, 전역 단축키를 눌렀을 때 즉각적으로 호출되고 첫 번째 키 입력부터 부드럽게 반응합니다.

---

## 📌 저장소 안내 (Repository Notice)

본 저장소(`sjstudio-app/jeppareu`)는 제빠르(Jeppareu)의 **공식 공개 배포(Releases) 및 사용자 기술 지원(Issues)**을 위한 창구입니다.

- **소프트웨어 라이선스 정책**: 제빠르는 SJ Studio가 개발한 **무료 독점 소프트웨어(Free Proprietary Software)**입니다. 오픈소스 라이선스(MIT, Apache, GPL 등)로 배포되지 않으며, **소스 코드는 비공개(Private)로 안전하게 관리**됩니다.
- **배포 창구**: 공식 빌드 패키지(`.zip`) 및 체크섬은 [GitHub Releases](https://github.com/sjstudio-app/jeppareu/releases)를 통해서만 공개 배포됩니다.
- **지원 및 피드백**: 버그 제보, 사용 문의, 기능 제안은 [GitHub Issues](https://github.com/sjstudio-app/jeppareu/issues)를 이용해 주시기 바랍니다.

---

## 🚀 주요 기능 (Core Features)

- **전역 단축키 즉시 호출**
  - <kbd>⌥</kbd> <kbd>Space</kbd>: 런처 열기 / 닫기
  - <kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>P</kbd>: 프로젝트 선택기 (VS Code로 프로젝트 즉시 열기)
  - <kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd>: 선택 영역 번역 (어느 앱에서든 선택한 텍스트를 독립 번역 패널에서 즉시 번역)
  - 세 전역 단축키는 상호 독립적이며, 별도 선행 단계 없이 즉시 전환됩니다.
- **네 가지 검색 모드 순환 (<kbd>⌘</kbd> <kbd>[</kbd>, <kbd>⌘</kbd> <kbd>]</kbd>)**
  - **All (통합)** ⇄ **Clipboard (클립보드)** ⇄ **Files (파일 시스템)** ⇄ **Translations (번역 기록)**
- **클립보드 기록 (Clipboard History)**
  - 텍스트, 이미지, 파일 복사 이력을 로컬 SQLite에 영구 보관하고 상주 메모리 기반으로 즉시 검색
  - 한글 초성 검색(Choseong Search) 완벽 지원
  - 자주 쓰는 항목 고정(<kbd>⌘</kbd> <kbd>P</kbd>) 및 섹션 이동(<kbd>⌥</kbd> <kbd>↑</kbd> 또는 <kbd>⌥</kbd> <kbd>↓</kbd>) (Pinned / History)
  - 서식 없이 붙여넣기(<kbd>⇧</kbd> <kbd>↵</kbd>), 항목 삭제(<kbd>⌘</kbd> <kbd>⌫</kbd>), 종류 필터(`text:`/`img:`/`file:`), 기간별 기록 삭제(15분/1시간/오늘)
  - 텍스트 미리보기 내 인라인 편집(<kbd>⌘</kbd> <kbd>E</kbd>) 및 검색(<kbd>⌘</kbd> <kbd>F</kbd>)
  - 여러 파일 복사 시 개별 파일명 단위 검색 매칭 및 미리보기 파일 넘기기(<kbd>⇧</kbd> <kbd>⌘</kbd> <kbd>[</kbd> 또는 <kbd>⇧</kbd> <kbd>⌘</kbd> <kbd>]</kbd>)
  - 연속 동일 복사 중복 방지, 민감 항목 메모리 보류(Sensitive Content), 특정 앱 기록 제외(Excluded Apps)
- **이미지 미리보기 (Image Preview, <kbd>⌘</kbd> <kbd>Y</kbd>)**
  - 클립보드 이미지 및 복사된 이미지 파일을 전용 검사 창에서 확인
  - 확대·축소(<kbd>⌘</kbd> <kbd>+</kbd> 또는 <kbd>⌘</kbd> <kbd>-</kbd>), 실제 크기(<kbd>⌘</kbd> <kbd>0</kbd>), 창 맞춤(<kbd>⌘</kbd> <kbd>9</kbd>), 패닝 및 다중 이미지 탐색(<kbd>←</kbd> 또는 <kbd>→</kbd>)
  - 미리보기 창에서 외부 앱으로 드래그 앤 드롭 지원
- **독립 번역 패널 및 번역 기록 (Translation)**
  - 전역 단축키(<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd>)로 호출되는 가볍고 독립적인 번역 패널
  - 클립보드 항목 번역(<kbd>⌘</kbd> <kbd>K</kbd> → `Translate This`)
  - 번역 기록(Translations 모드) 보관, 원문/번역문 언어 방향 전환(<kbd>⌘</kbd> <kbd>S</kbd>), 재번역(<kbd>⌘</kbd> <kbd>O</kbd>), 고정(<kbd>⌘</kbd> <kbd>P</kbd>), 삭제(<kbd>⌘</kbd> <kbd>⌫</kbd>), 원문 복사(<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>C</kbd>)
- **프로젝트 빠른 열기 (Project Open)**
  - 전용 전역 단축키(<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>P</kbd>)로 프로젝트 선택기를 호출하여 로컬 개발 프로젝트를 VS Code에서 즉시 오픈
- **파일 시스템 경로 및 자동완성 (Path Handling & Completion)**
  - `/` 또는 `~/` 경로 입력 시 <kbd>Tab</kbd> 키로 경로 자동완성 및 하위 파일/폴더 브라우징
  - 폴더 → Finder에서 열기, 파일 → 기본 앱 실행, 애플리케이션 → 즉시 실행
- **웹 세션 및 외부 검색 (External Actions)**
  - 검색어 입력 후 <kbd>Tab</kbd> 키로 웹 세션 진입 (맨 앞 키워드, 예: `g 검색어` → <kbd>Tab</kbd> 으로 제공자 지정)
  - 기본 10종 검색 제공자 지원 (Google, Naver, Google Maps, Daum, X, Naver Map, Kakao Map, Naver Shopping, Danawa, Naver Dictionary)
  - 이번 한 번만 열 브라우저 선택(웹 세션에서 <kbd>⌘</kbd> <kbd>K</kbd>) 및 사용자 맞춤 검색 제공자 추가/관리
- **단축키 안내 체계 (Keyboard Discoverability)**
  - 어느 화면에서든 <kbd>⌘</kbd> <kbd>/</kbd>를 눌러 현재 화면의 단축키 치트시트 팝오버 확인
  - 런처 하단 28pt 푸터(Footer)에서 현재 상황에 맞는 핵심 단축키 실시간 안내
- **Local-First & 프라이버시 보호**
  - 모든 클립보드 이력과 데이터는 사용자 Mac 내 로컬에만 안전하게 저장됩니다.
  - 외부 통신, 클라우드 동기화, 사용자 분석 텔레메트리 SDK를 일체 포함하지 않습니다.

---

## ⌨️ 주요 단축키 (Keyboard Shortcuts)

> 💡 앱 내 어느 화면에서든 <kbd>⌘</kbd> <kbd>/</kbd>를 누르면 현재 화면에서 사용할 수 있는 단축키 치트시트가 표시됩니다.

### 전역 단축키

| 키 | 동작 |
|---|---|
| <kbd>⌥</kbd> <kbd>Space</kbd> | 런처 열기 / 닫기 (Settings → General 에서 변경) |
| <kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>P</kbd> | 프로젝트 선택기 열기 (Settings → Projects 에서 변경·해제) |
| <kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd> | 선택 영역 번역 패널 열기 (Settings → General 에서 변경·해제) |
| <kbd>⌘</kbd> <kbd>,</kbd> | 설정 창 열기 |
| <kbd>⌘</kbd> <kbd>/</kbd> | 현재 화면 단축키 도움말 |

### 런처 (<kbd>⌥</kbd> <kbd>Space</kbd>)

| 키 | 동작 |
|---|---|
| <kbd>↑</kbd> / <kbd>↓</kbd> | 결과 선택 이동 |
| <kbd>Return</kbd> | 선택한 결과 실행 (기본 동작: 앱 실행 / 파일 열기 / 클립보드 붙여넣기) |
| <kbd>⌘</kbd> <kbd>1–9</kbd> | 상위 1~9번째 결과 즉시 실행 |
| <kbd>⌘</kbd> <kbd>[</kbd> 또는 <kbd>⌘</kbd> <kbd>]</kbd> | 검색 모드 순환 (All ⇄ Clipboard ⇄ Files ⇄ Translations) |
| <kbd>⌘</kbd> <kbd>P</kbd> | 클립보드 / 번역 항목 고정(Pin) 전환 |
| <kbd>⌥</kbd> <kbd>↑</kbd> 또는 <kbd>⌥</kbd> <kbd>↓</kbd> | 섹션 이동 (Pinned ⇄ History, 검색어가 비어 있을 때) |
| <kbd>⌘</kbd> <kbd>Y</kbd> | 이미지 미리보기 창 열기 |
| <kbd>⌘</kbd> <kbd>K</kbd> | 선택 항목 추가 액션 메뉴 |
| <kbd>⌘</kbd> <kbd>R</kbd> | Finder에서 보기 (Reveal in Finder) |
| <kbd>⌘</kbd> <kbd>C</kbd> | 텍스트 복사 / 경로 복사 (붙여넣지 않고 클립보드에 복사) |
| <kbd>⇧</kbd> <kbd>↵</kbd> | 텍스트 클립보드 항목을 서식 없이 붙여넣기 |
| <kbd>⌘</kbd> <kbd>⌫</kbd> | 선택한 클립보드 항목 삭제 |
| <kbd>Tab</kbd> | 경로 자동완성 (경로 입력 시) / 웹 세션 진입 (일반 검색어 입력 시) |
| <kbd>Esc</kbd> | 한 단계 뒤로 / 액션 메뉴 닫기 / 런처 닫기 |
| <kbd>⌘</kbd> <kbd>Q</kbd> | Jeppareu 종료 |

### 클립보드 미리보기 편집 및 검색 (미리보기 포커스 시)

| 키 | 동작 |
|---|---|
| <kbd>⌘</kbd> <kbd>F</kbd> | 미리보기 텍스트 안에서 찾기 |
| <kbd>⌘</kbd> <kbd>E</kbd> | 미리보기 텍스트 인라인 편집 |
| <kbd>⌘</kbd> <kbd>Enter</kbd> | 편집한 텍스트를 새 클립보드 값으로 확정 복사 |
| <kbd>Esc</kbd> | 찾기 닫기 / 편집 취소 / 검색창으로 포커스 복귀 |

### 이미지 미리보기 (<kbd>⌘</kbd> <kbd>Y</kbd>)

| 키 | 동작 |
|---|---|
| <kbd>⌘</kbd> <kbd>+</kbd> 또는 <kbd>⌘</kbd> <kbd>-</kbd> | 확대 / 축소 |
| <kbd>⌘</kbd> <kbd>0</kbd> 또는 <kbd>⌘</kbd> <kbd>9</kbd> | 실제 크기 (100%) / 창 크기에 맞춤 |
| <kbd>←</kbd> 또는 <kbd>→</kbd> | 이전 / 다음 이미지 (여러 장 복사 시) |
| `드래그` | 외부 앱으로 이미지 파일 드래그 앤 드롭 |
| <kbd>Space</kbd> 또는 <kbd>Esc</kbd> | 미리보기 창 닫기 |

### 번역 패널 (<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd>)

| 키 | 동작 |
|---|---|
| <kbd>⌘</kbd> <kbd>S</kbd> | 원문 언어와 번역 언어 방향 바꾸고 다시 번역 |
| <kbd>⌘</kbd> <kbd>C</kbd> | 번역된 텍스트를 클립보드에 복사 |
| <kbd>Esc</kbd> 또는 <kbd>⌘</kbd> <kbd>W</kbd> | 번역 패널 닫고 이전 작업 앱으로 복귀 |

---

## 📥 다운로드 및 설치 (Download & Installation)

1. [GitHub Releases](https://github.com/sjstudio-app/jeppareu/releases)에서 최신 버전의 `Jeppareu-<VERSION>.zip`을 다운로드합니다.
2. 압축을 풀고 `Jeppareu.app`을 `/Applications` (응용 프로그램) 폴더로 이동합니다.
3. 앱을 실행하고 화면의 안내에 따라 **손쉬운 사용 (Accessibility)** 권한을 허용합니다. (런처 항목 선택 시 직전 작업 앱으로 자동 붙여넣기를 실행하는 데 필요합니다.)
4. <kbd>⌥</kbd> <kbd>Space</kbd>를 눌러 런처를 실행합니다.

> **시스템 요구사항**:
> - Apple Silicon Mac (M1 / M2 / M3 / M4)
> - macOS 15.0 (Sequoia) 이상
> - Apple Developer ID 정식 코드 서명 및 Apple Notarization(공증) 완료

---

## 📖 문서 및 정책 (Documentation & Policies)

- [사용자 가이드 및 지원 안내 (SUPPORT.md)](SUPPORT.md)
- [개인정보 처리방침 (PRIVACY.md)](PRIVACY.md)
- [최종 사용자 사용권 계약 (EULA.md)](EULA.md)

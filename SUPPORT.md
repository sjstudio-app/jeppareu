# 제빠르 (Jeppareu) 지원 및 사용자 가이드

제빠르(Jeppareu)의 공식 지원 채널 및 사용자 가이드입니다.

---

## 1. 공식 지원 채널

제빠르의 공식 지원 및 피드백 접수 창구는 **GitHub Issues**입니다.

- **이슈 트래커 (버그 신고 / 기능 제안)**:
  [https://github.com/sjstudio-app/jeppareu/issues](https://github.com/sjstudio-app/jeppareu/issues)

---

## 2. 사용자 가이드 (Getting Started)

### 앱 실행 및 백그라운드 상주
- 설치 후 `Jeppareu.app`을 실행하면 Dock에 아이콘이 상주하지 않고 백그라운드 액세서리 프로세스로 대기합니다.
- 메뉴 막대에는 기본으로 제빠르 아이콘이 표시되며, 환경설정 **General** 탭의 `Show in menu bar`로 숨길 수 있습니다.
- 실행 중 언제든지 전역 단축키를 눌러 런처를 즉시 호출할 수 있습니다. 앱을 끝내려면 런처에서 <kbd>⌘</kbd> <kbd>Q</kbd>를 누르거나 General 탭의 `Quit Jeppareu`를 누릅니다.

### 런처 전역 단축키 (<kbd>⌥</kbd> <kbd>Space</kbd>)
- 기본 단축키: **<kbd>⌥</kbd> <kbd>Space</kbd> (Option-Space)**
- 단축키를 누르면 화면 중앙에 즉시 런처 입력창이 나타나며 텍스트 입력 포커스를 획득합니다.
- 런처가 열려 있는 상태에서 다시 <kbd>⌥</kbd> <kbd>Space</kbd>를 누르거나 <kbd>Esc</kbd> 키를 누르면 런처가 닫힙니다.
- 환경설정(<kbd>⌘</kbd> <kbd>,</kbd>)에서 원하는 키 조합으로 언제든지 변경할 수 있습니다.

### 프로젝트 피커 전역 단축키 (<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>P</kbd>)
- 기본 단축키: **<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>P</kbd> (Option-Command-P)**
- 런처와는 **별개의 독립 단축키**입니다. 런처를 먼저 띄우거나 검색 모드를 순환할 필요 없이, 곧바로 프로젝트 피커가 열립니다.
- 반대로 프로젝트 피커가 떠 있을 때 <kbd>⌥</kbd> <kbd>Space</kbd>를 누르면 일반 검색으로 전환됩니다. 두 세션은 서로 배타적입니다.
- 환경설정 **Projects** 탭에서 키 조합을 바꾸거나, 기능 자체를 끌 수 있습니다. 껐다가 다시 켜도 직접 지정한 키는 그대로 보존됩니다.

### 선택 영역 번역 전역 단축키 (<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd>)
- 기본 단축키: **<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd> (Option-Command-T)**
- 런처와는 **별개의 독립 단축키**입니다. 어느 앱에서든 텍스트를 마우스나 키보드로 선택한 후 <kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd>를 누르면 가볍고 독립적인 번역 패널이 즉시 나타나 번역 결과를 표시합니다.
- 선택한 텍스트가 없거나 대상 앱이 텍스트 읽기를 지원하지 않는 경우, 클립보드에 복사된 최근 텍스트로 자동 대체(fallback)하여 번역을 수행합니다.
- 번역 패널 안에서 <kbd>⌘</kbd> <kbd>S</kbd>로 원문과 번역문 언어 방향을 바꾸고, <kbd>⌘</kbd> <kbd>C</kbd>로 번역된 텍스트를 복사할 수 있으며, <kbd>Esc</kbd> 또는 <kbd>⌘</kbd> <kbd>W</kbd>로 패널을 닫고 이전 작업 앱으로 복귀합니다.
- 런처 및 프로젝트 피커와는 **상호 배타적**이며, 환경설정 **General** 탭에서 단축키를 변경하거나 기능을 끌 수 있습니다.

### 네 가지 검색 모드 전환 (<kbd>⌘</kbd> <kbd>[</kbd>, <kbd>⌘</kbd> <kbd>]</kbd>) 및 사전 접두어 라우팅 (`?`)
런처가 열린 상태에서 다음 단축키를 눌러 검색 범위를 순환 전환할 수 있습니다:
- **<kbd>⌘</kbd> <kbd>[</kbd>** : 이전 모드로 전환
- **<kbd>⌘</kbd> <kbd>]</kbd>** : 다음 모드로 전환
- 순환 순서: **All** ⇄ **Clipboard** ⇄ **Files** ⇄ **Translations** ⇄ **All**
- 모드를 전환해도 현재 입력창에 작성 중인 검색어는 유지되며, 검색 결과만 즉각적으로 업데이트됩니다.
- 프로젝트 피커와 번역 패널은 이 순환에 포함되지 않는 독립 세션이므로, 해당 화면에서는 <kbd>⌘</kbd> <kbd>[</kbd> / <kbd>⌘</kbd> <kbd>]</kbd>가 동작하지 않습니다.
- **사전 접두어 라우팅 (`?`)**: 검색창에 `?`를 입력하면 모드 순환을 변경하지 않고도 사전 접두어 쿼리 모드에 즉시 진입하며, 런처 좌측 뱃지가 `Dictionary` 칩 뱃지로 바뀝니다. `?`를 지우거나 검색어를 비우면 직전 검색 모드로 자동 복귀합니다.

### 추가 작업 액션 메뉴 (<kbd>⌘</kbd> <kbd>K</kbd>)
- 검색 결과 목록에서 특정 항목을 선택한 후 **<kbd>⌘</kbd> <kbd>K</kbd>**를 누르면 해당 항목이 지원하는 추가 액션 메뉴가 열립니다.
- 액션 메뉴 내에서 <kbd>↑</kbd> / <kbd>↓</kbd> 방향키로 액션을 탐색하고 <kbd>Return</kbd>으로 실행하거나, <kbd>Esc</kbd> 또는 일반 문자를 입력하여 액션 메뉴를 닫고 검색으로 돌아올 수 있습니다.
- **클립보드 항목 액션**: Paste (기본, <kbd>Return</kbd>), Copy to Clipboard (<kbd>⌘</kbd> <kbd>C</kbd>), Paste as Plain Text (<kbd>⇧</kbd> <kbd>↵</kbd>, 텍스트 항목), Translate This (텍스트 항목 번역), Open Preview, Delete from Clipboard History (<kbd>⌘</kbd> <kbd>⌫</kbd>), `Clear Last 15 Minutes…` / `Clear Last Hour…` / `Clear Today…`. 보류 중인 민감 항목에는 `Keep in History…`가 나타납니다.
- **파일 항목 액션**: Open / Open Directory / Launch Application (기본, <kbd>Return</kbd>), Reveal in Finder (<kbd>⌘</kbd> <kbd>R</kbd>), Copy Path (<kbd>⌘</kbd> <kbd>C</kbd>), Open With….
- **사전 항목 액션**: 뜻풀이 붙여넣기 (기본, <kbd>Return</kbd>), 뜻풀이 복사 (<kbd>⌘</kbd> <kbd>C</kbd>), 사전 앱에서 열기 (<kbd>⌥</kbd> <kbd>Return</kbd> 또는 <kbd>⌘</kbd> <kbd>O</kbd>), 사전 기록에서 삭제 (<kbd>⌘</kbd> <kbd>⌫</kbd>, 히스토리 항목), 전체 사전 기록 삭제 (`Clear All Dictionary History…`).
- 외부 검색 제공자는 <kbd>⌘</kbd> <kbd>K</kbd> 메뉴에 나오지 않습니다. 웹 검색은 <kbd>Tab</kbd>으로 들어가는 웹 세션에서 합니다(아래 「외부 검색」).
- 프로젝트 피커에서는 <kbd>⌘</kbd> <kbd>K</kbd>가 동작하지 않습니다. 프로젝트는 <kbd>Return</kbd>으로 VS Code에서 열고, <kbd>⌘</kbd> <kbd>R</kbd>로 Finder에서 보거나 <kbd>⌘</kbd> <kbd>C</kbd>로 폴더 경로를 복사할 수 있습니다.

### 환경설정 (<kbd>⌘</kbd> <kbd>,</kbd>)
런처가 활성화된 상태에서 **<kbd>⌘</kbd> <kbd>,</kbd>** (또는 앱 메뉴의 Settings)를 누르면 네이티브 설정 창이 열립니다. 탭은 네 개입니다.

- **General 탭**:
  - `Launcher Shortcut`: 새로운 단축키를 입력하여 등록. 시스템 단축키와 충돌 시 경고 메시지가 표시되며 이전 단축키로 안전하게 롤백됩니다.
  - `Default Search Mode`: 런처를 새로 호출할 때 기본으로 열릴 검색 모드(All, Clipboard, Files, Translations)를 지정합니다.
  - `Show in menu bar`: 메뉴 막대 아이콘 표시 여부(기본 켜짐). `Quit Jeppareu` 버튼으로 앱을 종료합니다.
  - `Translation`: 번역 엔진(Automatic, Apple Intelligence, System Translation, Off)과 선택 영역 번역 단축키(기본 <kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd>)의 변경 및 사용 여부를 설정합니다.
  - `Open Searches In` (Web Search): 외부 검색을 열 기본 브라우저를 지정합니다. macOS 기본 브라우저와 이 Mac에 설치된 브라우저만 목록에 나옵니다. 이미 골라 둔 브라우저를 지우면 목록에 `(not installed)`로 남습니다. 목록에 없는 브라우저는 아래 `Custom Browsers`의 `Add Browser…`로 `.app`을 골라 추가합니다. 웹 페이지(`http`/`https`)를 열지 못하는 앱이나 이미 목록에 있는 브라우저는 추가되지 않습니다. 기본 브라우저로 쓰던 사용자 추가 브라우저를 제거하면 macOS 기본 브라우저로 돌아갑니다.
  - `Window Position`: 런처가 처음 나타날 디스플레이(마우스가 있는 화면 / 주 디스플레이)와 세로 위치(Upper Center, Center, Top, Custom)를 지정합니다. `Remember window position when moved`를 켜면 옮긴 위치를 기억합니다.
- **Clipboard 탭**:
  - `Keep History`: 클립보드 보관 기간(7 Days, 30 Days, 90 Days, 1 Year, Unlimited) 설정. 기본값은 Unlimited입니다.
  - `Maximum Items`: 최대 보관 개수(100 Items, 500 Items, 1,000 Items, 5,000 Items, 10,000 Items, Unlimited) 설정. 기본값은 Unlimited입니다. 고정 항목은 자동으로 지워지지 않습니다.
  - `Sensitive Content`: 비밀번호 관리자 등이 민감하다고 표시한 복사본을 디스크에 저장하지 않고 메모리에만 잠시 보류합니다(기본 켜짐). `Forget held items after`로 보류 시간(30 seconds, 2 minutes, 10 minutes)을 정하고, `Remove Saved Sensitive Items…`로 이미 저장된 민감 항목을 찾아 지웁니다.
  - `Excluded Apps`: `Add App…`으로 고른 앱이 앞에 있을 때 복사한 내용은 기록하지 않습니다.
  - `Clear History…`: `Last 15 Minutes…` / `Last Hour…` / `Today…`는 그 시간 범위의 기록만 지웁니다(고정 항목은 남김). 같은 항목이 런처의 클립보드 행 <kbd>⌘</kbd> <kbd>K</kbd> 메뉴에도 있습니다. `All History…`는 고정 항목을 포함해 모든 클립보드 메타데이터와 페이로드 파일을 즉시 영구 삭제합니다. 어느 쪽이든 확인을 거칩니다.
- **Projects 탭**:
  - `Enable project shortcut`: 프로젝트 피커 전역 단축키의 사용 여부. 끄면 키 조합이 다른 앱에 반환되며, 런처 단축키에는 영향을 주지 않습니다.
  - `Project Shortcut`: 프로젝트 피커를 여는 키 조합(기본 <kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>P</kbd>).
  - `Projects`: 등록된 프로젝트 목록. `Add Project…`를 누르면 macOS 폴더 선택 창이 열리고, 선택한 디렉터리가 폴더 이름을 표시 이름으로 하여 등록됩니다. 각 행의 `–` 버튼으로 등록을 해제합니다.
- **Search 탭**:
  - `Custom Providers`: 사용자 정의 외부 검색 제공자를 추가·수정·삭제하고, 켜고 끄거나 순서를 바꿉니다.
  - `Built-in Providers`: 내장 제공자와 예약된 트리거 키워드를 읽기 전용으로 보여줍니다.

---

## 3. 핵심 기능 워크플로우

### 클립보드 히스토리 사용 (Clipboard Usage)
1. 텍스트나 이미지를 복사하면 제빠르가 백그라운드에서 자동으로 히스토리에 기록합니다.
2. <kbd>⌥</kbd> <kbd>Space</kbd>로 런처를 열고 검색어를 입력하면 과거 복사한 내용을 빠르게 찾을 수 있습니다.
3. 원하는 항목에서 **<kbd>Return</kbd>**을 누르면 런처가 닫히고, 런처를 열기 직전에 사용 중이던 앱으로 돌아가 해당 항목을 자동으로 붙여넣습니다.
4. **<kbd>⌘</kbd> <kbd>1–9</kbd>** 단축키를 눌러 상위 9개 결과를 즉시 붙여넣을 수도 있습니다.
5. 복사만 하고 붙여넣지는 않으려면 <kbd>⌘</kbd> <kbd>K</kbd> > `Copy to Clipboard`(또는 <kbd>⌘</kbd> <kbd>C</kbd>)를 선택합니다.

### 파일 시스템 검색 및 직접 경로 입력 (Files Search)
- **직접 경로 입력 (Direct Path)**:
  - `/`로 시작하는 절대 경로(예: `/Applications`, `/Library`) 또는 `~`로 시작하는 홈 디렉터리 경로(예: `~/Downloads`, `~/Documents`)를 입력하면 즉시 유효성을 검사하여 최상단에 고정 표시합니다.
- **Spotlight 비동기 파일명 검색**:
  - 일반 파일명이나 디렉터리명을 입력하면 시스템 Spotlight 인덱스를 통해 백그라운드에서 실시간으로 결과를 찾아 매칭 및 하이라이트합니다.
- **실행 동작**:
  - 디렉터리: Finder에서 해당 폴더를 엽니다.
  - 일반 파일: macOS 기본 연결 애플리케이션으로 파일을 엽니다.
  - 애플리케이션(`.app`): 해당 앱을 즉시 실행합니다.

### 프로젝트 열기 (Project Open)
1. 환경설정 **Projects** 탭에서 `Add Project…`로 자주 쓰는 프로젝트 디렉터리를 먼저 등록합니다. 위치 제한은 없으며, `~/code` 아래가 아니어도 됩니다.
2. <kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>P</kbd>를 누르면 프로젝트 목록이 즉시 나타나고 첫 항목이 선택되어 있습니다.
3. 검색어를 입력하면 프로젝트 이름과 경로를 대상으로 즉시 필터링됩니다. 초성 검색과 부분 일치가 그대로 적용됩니다.
4. <kbd>Return</kbd>(또는 <kbd>⌘</kbd> <kbd>1–9</kbd>)을 누르면 선택한 디렉터리가 **Visual Studio Code**에서 열립니다. VS Code Insiders, VSCodium 등 다른 변형은 지원하지 않습니다.
5. 성공적으로 연 프로젝트는 **Recent**로 기록되어 다음 호출 때 위쪽에 먼저 나타납니다. 열기에 실패하면 Recent 순서는 바뀌지 않습니다.
6. 오른쪽 상세 영역에는 프로젝트 이름, 절대 경로, 마지막으로 연 시각이 표시됩니다.
7. 등록된 프로젝트도 Recent 기록도 없으면 `No Projects — Add a project in Settings` 안내가 표시됩니다. 이때 클립보드나 파일 결과로 대체되지는 않습니다.
8. 제빠르는 프로젝트를 자동으로 탐색하지 않습니다. 디스크를 뒤지거나 Git 상태·브랜치를 조회하지 않으며, 목록은 사용자가 등록했거나 실제로 연 프로젝트로만 구성됩니다.

### 번역 및 번역 히스토리 (Translation & History)

제빠르는 시스템 내장 번역 엔진을 활용하여 외부 네트워크 전송 없이 빠르고 안전한 번역을 제공합니다.

- **선택 영역 즉시 번역 (<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd>)**:
  - 어느 앱에서든 번역하고 싶은 텍스트를 선택한 후 <kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd>를 누르면 전용 번역 패널이 열립니다.
  - 선택 영역이 없거나 대상 앱이 텍스트 접근을 지원하지 않는 경우 클립보드의 최근 텍스트를 자동으로 대체 번역합니다.
  - <kbd>⌘</kbd> <kbd>S</kbd>: 원문과 번역문의 언어 방향을 전환하고 다시 번역합니다.
  - <kbd>⌘</kbd> <kbd>C</kbd>: 번역된 결과를 클립보드에 복사합니다.
  - <kbd>Esc</kbd> / <kbd>⌘</kbd> <kbd>W</kbd>: 번역 패널을 닫고 이전 앱으로 복귀합니다.
- **클립보드 항목 번역**:
  - 런처(<kbd>⌥</kbd> <kbd>Space</kbd>)에서 텍스트 항목을 선택한 뒤 <kbd>⌘</kbd> <kbd>K</kbd> > `Translate This`를 누르면 즉시 번역 결과가 오버레이됩니다.
- **번역 히스토리 (Translations 검색 모드)**:
  - 번역된 결과는 로컬 Translation History에 자동 기록됩니다.
  - 런처에서 <kbd>⌘</kbd> <kbd>[</kbd> / <kbd>⌘</kbd> <kbd>]</kbd>를 눌러 **Translations** 모드로 전환하면 과거 번역 이력을 원문 및 번역문으로 검색할 수 있습니다 (All 검색에는 자동으로 섞이지 않습니다).
  - <kbd>Return</kbd>: 번역문을 직전 앱에 붙여넣기
  - <kbd>⌘</kbd> <kbd>C</kbd>: 번역문 복사 후 런처 닫기
  - <kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>C</kbd>: 원문 복사
  - <kbd>⌘</kbd> <kbd>S</kbd>: 언어 방향 전환
  - <kbd>⌘</kbd> <kbd>O</kbd>: 다시 번역
  - <kbd>⌘</kbd> <kbd>P</kbd>: 번역 항목 고정(Pin) 토글
  - <kbd>⌘</kbd> <kbd>⌫</kbd>: 번역 항목 삭제

### 이미지 프리뷰 (Image Preview)

- 이미지 클립보드 항목을 선택하면 상세 영역에서 이미지 프리뷰가 표시됩니다.
- <kbd>⌘</kbd> <kbd>Y</kbd> 또는 프리뷰의 검사 버튼으로 전용 이미지 검사 창을 열 수 있습니다.
- 트랙패드 pinch gesture로 확대·축소하고 두 손가락으로 확대된 이미지를 이동할 수 있습니다. 검사 창에서 <kbd>⌘</kbd> <kbd>C</kbd>를 누르면 보고 있는 이미지를 복사합니다.
- 프리뷰에는 픽셀 크기, 포맷, 파일 크기가 표시됩니다.
- 프리뷰 이미지는 다른 앱으로 드래그하여 파일로 전달할 수 있습니다.
- 원본 이미지 데이터가 있으면 drag export는 재인코딩하지 않고 원본 바이트를 그대로 사용합니다.

### 사전 검색 및 백과사전 (Dictionary)

런처 검색창에서 `?` 접두어를 입력하면 모드 전환 단축키 없이도 인라인 사전 검색 환경으로 즉시 진입합니다.

- **최근 조회한 사전 단어 기록 (`?` 단독 입력)**:
  - `?`만 입력하면 최근에 조회하고 복사/붙여넣기했던 사전 단어 기록(`DictionaryHistoryStore`)을 최신순으로 최대 200개까지 탐색할 수 있습니다.
  - 선택한 행의 뜻풀이가 우측 프리뷰에 즉시 표시됩니다.
- **로컬 사전 저지연 검색 (`?<단어>`)**:
  - `?` 뒤에 검색할 단어를 입력하면 macOS 로컬 사전(`DictionaryServices`)을 통해 국어사전, 영한/한영사전 표제어와 뜻풀이를 50ms 미만의 극히 낮은 지연 시간으로 실시간 검색합니다.
  - 메인 스레드를 차단하지 않는 백그라운드 액터 격리와 플레인 텍스트 정규화 파서를 통해 타이핑 반응성을 완벽히 보장합니다.
  - 검색 결과 목록의 최하단에는 정적 검색 행인 `[위키백과] '<단어>' 검색`이 항상 함께 제공됩니다.
- **위키백과 온디맨드 로딩**:
  - 사용자가 타이핑하는 동안에는 어떠한 외부 네트워크 요청도 발생하지 않습니다(0 request).
  - 결과 목록에서 사용자가 위키백과 행을 방향키로 명시적으로 선택(하이라이트)했을 때만 프리뷰에서 Wikimedia REST API를 통해 비동기로 표제어 요약문과 썸네일을 로드합니다.
  - 다른 행으로 이동하거나 검색어를 변경하면 진행 중이던 비동기 요청은 안전하게 무시됩니다.
- **단축키 및 인터랙션**:
  - <kbd>Return</kbd>: 현재 활성 앱에 표제어 및 대표 뜻풀이를 즉시 붙여넣고 런처를 닫습니다.
  - <kbd>⌘</kbd> <kbd>C</kbd>: 전체 표제어 및 상세 정의 텍스트를 클립보드에 복사하고 런처를 닫습니다.
  - <kbd>⌥</kbd> <kbd>Return</kbd> 또는 <kbd>⌘</kbd> <kbd>O</kbd>: macOS 사전 앱(Dictionary.app)을 열어 시스템 전체 사전에서 단어를 확인합니다 (`dict://`).
  - <kbd>⌘</kbd> <kbd>⌫</kbd>: 선택한 사전 기록 항목을 히스토리에서 즉시 삭제합니다.
- **기록 저장 시점 (Save-on-use)**:
  - 검색 결과에 대해 <kbd>Return</kbd>(붙여넣기) 또는 <kbd>⌘</kbd> <kbd>C</kbd>(복사)를 실행한 시점에만 히스토리에 영구 저장됩니다.
  - 단순 타이핑, 훑어보기, 오타 검색, 위키백과 행 선택 등은 기록되지 않습니다.
- **외부 웹 사전(`dict` 키워드)과의 차이점**:
  - `dict <단어>` 입력 후 <kbd>Tab</kbd>을 누르는 External Actions는 기본 웹 브라우저를 통해 네이버 사전 웹페이지를 여는 외부 액션입니다.
  - 반면 `?<단어>`는 제빠르 런처 내에서 macOS 로컬 사전 데이터를 활용해 즉시 뜻풀이를 인라인 확인하고 본문에 붙여넣는 네이티브 기능입니다.

### 외부 검색 (External Actions)
검색어를 웹 검색·지도·쇼핑·사전 서비스로 보내 원하는 브라우저에서 엽니다. 제빠르 안에 웹 화면을 띄우지 않고, 열기는 macOS에 위임합니다.

**웹 세션 들어가기 (<kbd>Tab</kbd>)**

검색어를 입력한 상태에서 <kbd>Tab</kbd>을 누르면 웹 세션에 들어갑니다. 목록의 각 행은 검색 제공자이며, <kbd>↑</kbd> / <kbd>↓</kbd>로 고르고 <kbd>Return</kbd>을 누르면 그 제공자로 검색어를 브라우저에서 엽니다. <kbd>⌘</kbd> <kbd>1–9</kbd>로 해당 자리의 제공자로 바로 검색할 수도 있습니다.

검색어 맨 앞에 제공자 키워드를 쓰고 <kbd>Tab</kbd>을 누르면 그 제공자가 지정된 상태로 들어갑니다. 예: `g cats` → <kbd>Tab</kbd>, `n 고양이` → <kbd>Tab</kbd>, `maps 판교역` → <kbd>Tab</kbd>.

| 키워드 | 제공자 | | 키워드 | 제공자 |
|---|---|---|---|---|
| `g` | Google | | `nmap` | Naver Map |
| `n` | Naver | | `kmap` | Kakao Map |
| `maps` | Google Maps | | `ns` | Naver Shopping |
| `d` | Daum | | `dn` | Danawa |
| `x` | X | | `dict` | Naver Dictionary |

- <kbd>Tab</kbd>을 누르기 전까지 `g cats` 같은 입력은 일반 검색어입니다. 키워드와 공백만으로는 외부 검색이 실행되지 않습니다.
- 키워드가 지정된 상태에서 입력란을 비우고 <kbd>⌫</kbd>를 누르면 모든 제공자가 다시 보이고, 한 번 더 누르면 웹 세션을 나갑니다.
- <kbd>Esc</kbd>를 누르면 웹 세션을 나가 들어오기 전의 검색 모드로 돌아갑니다. 웹 세션 안에서 <kbd>Tab</kbd> 또는 <kbd>⇧</kbd> <kbd>Tab</kbd>을 누르면 입력한 텍스트를 그대로 둔 채 돌아갑니다.
- `/`나 `~`로 시작하는 경로 입력에서는 <kbd>Tab</kbd>이 경로 자동완성으로 동작합니다.
- 외부 검색 제공자는 <kbd>⌘</kbd> <kbd>K</kbd> 액션 메뉴에 나타나지 않습니다.

**브라우저 선택 (<kbd>⌘</kbd> <kbd>K</kbd>)**

- 웹 세션에서 제공자 행을 고른 뒤 <kbd>⌘</kbd> <kbd>K</kbd>를 누르면 그 검색을 열 수 있는 설치된 브라우저 목록이 나타납니다.
- 여기서 고른 브라우저는 **이번 실행에만** 적용되며 설정에 저장되지 않습니다. 기본 브라우저를 바꾸려면 General 탭의 `Open Searches In`을 사용합니다.
- 우선순위: 이번 실행에서 고른 브라우저 → General 탭의 설정 → macOS 기본 브라우저.
- 설치되어 있지 않은 브라우저는 목록에 나타나지 않습니다.

**사용자 정의 제공자**

환경설정 **Search** 탭의 `Add Provider…`에서 직접 추가합니다.
- `Name`: 웹 세션 목록에 표시할 이름.
- `Keyword`: 제공자 키워드(선택). 키워드를 쓰고 <kbd>Tab</kbd>을 누르면 이 제공자가 지정됩니다. 비워두면 웹 세션 목록에서 직접 고릅니다.
- `Address`: `{query}`가 정확히 한 번 들어간 `https` 주소. 예: `https://example.com/search?q={query}`.
- `Kind`: Search / Map / Shopping / Dictionary.

내장 제공자의 식별자와 키워드는 예약되어 있어 같은 값으로는 저장되지 않으며, 거절 사유가 시트에 표시됩니다.
`http://` 주소는 현재 정책상 허용되지 않고, `javascript:`·`file:` 같은 주소는 안전하지 않은 것으로 거부됩니다.

외부 검색은 프로젝트 피커에서는 사용할 수 없습니다.

---

## 4. macOS 권한 설정 (Accessibility Permission)

### 자동 붙여넣기에 손쉬운 사용(Accessibility) 권한이 필요한 이유
- 제빠르는 런처에서 항목을 선택했을 때 사용자가 직전에 작업하던 앱으로 포커스를 전환한 뒤 키보드 붙여넣기(<kbd>⌘</kbd> <kbd>V</kbd>) 이벤트를 전달합니다.
- macOS 보안 정책상 다른 애플리케이션에 키보드 이벤트를 전송하려면 **손쉬운 사용(Accessibility)** 권한이 필수적입니다.

### 권한 부여 방법
1. 앱 최초 실행 시 나타나는 **Permission Setup** 온보딩 창에서 `[Open System Settings]`를 클릭하거나, 직접 macOS **시스템 설정 (System Settings)**을 엽니다.
2. **개인정보 보호 및 보안 (Privacy & Security)** > **손쉬운 사용 (Accessibility)**으로 이동합니다.
3. 목록에서 **Jeppareu**를 찾아 스위치를 켭니다 (잠금이 되어 있다면 Mac 암호 또는 Touch ID 입력 필요).
4. 시스템 설정에서 스위치를 켠 뒤 앱 창으로 복귀하면 실시간으로 감지되어 화면이 🟢 **Accessibility Permission Granted** 및 단축키 안내로 자동 전환됩니다. `[Get Started]`(또는 Return 키)를 눌러 온보딩을 완료합니다.
5. 권한을 부여하지 않아도 런처 호출, 파일 검색, 클립보드 히스토리 검색, 수동 복사(<kbd>⌘</kbd> <kbd>C</kbd>), 애플리케이션 실행, 프로젝트 열기(<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>P</kbd>), 외부 검색은 정상 작동합니다. 선택 영역 번역(<kbd>⌥</kbd> <kbd>⌘</kbd> <kbd>T</kbd>)은 권한이 없으면 다른 앱의 선택 텍스트를 읽을 수 없어, 선택한 글 대신 최근에 복사한 텍스트를 번역합니다. 권한이 없을 때 할 수 없는 것은 <kbd>Return</kbd> 키를 통한 대상 앱으로의 자동 붙여넣기입니다.

---

## 5. 버그 신고 및 기능 제안 가이드

### 버그 신고 (Bug Report)
문제가 발생한 경우 [GitHub Issues](https://github.com/sjstudio-app/jeppareu/issues)에서 **New Issue**를 생성해 주세요. 빠른 원인 파악을 위해 다음 정보를 포함해 주시면 도움이 됩니다:

1. **macOS 버전**: (예: macOS 15.0 Sequoia, Apple Silicon M1/M2/M3/M4)
2. **증상 설명**: 기대했던 동작과 실제로 발생한 현상
3. **재현 단계**: 문제를 재현할 수 있는 구체적인 순서
4. **손쉬운 사용 권한 부여 여부**: 허용됨 / 허용되지 않음

### 기능 제안 (Feature Request)
제품 사용 중 유용하다고 생각되는 워크플로우나 기능 개선 아이디어가 있다면 언제든지 [GitHub Issues](https://github.com/sjstudio-app/jeppareu/issues)에 등록해 주시기 바랍니다.

- 어떤 상황에서 해당 기능이 필요한지
- 기존 도구(Raycast, Spotlight 등)와 비교했을 때 개선하고자 하는 작업 흐름

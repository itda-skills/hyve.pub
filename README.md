# hyve

> **공식 배포 채널** — 스킬.잇다 교육 과정 수강생을 위한 hyve 소프트웨어의 공개 릴리즈 저장소입니다.

<!-- CI-managed:start — 아래 항목은 itda-skills/hyve 의 GitHub Actions (release.yml) 이 자동으로 갱신합니다. 수동 편집 금지. -->

- **최신 버전**: `v0.10.0`

<!-- CI-managed:end -->

---

## 다운로드

모든 릴리즈 asset 은 GitHub Releases 에서 제공되며, CDN 302 redirect 로 안정적으로 전달됩니다.

| 플랫폼 | 파일 | 직링크 |
|--------|------|--------|
| Windows (x64 / ARM64) | `hyve-setup-windows-amd64.exe` | [최신 릴리즈로 이동](https://github.com/itda-skills/hyve.pub/releases/latest/download/hyve-setup-windows-amd64.exe) |
| SHA-256 체크섬 | `checksums.txt` | [최신 릴리즈로 이동](https://github.com/itda-skills/hyve.pub/releases/latest/download/checksums.txt) |
| 버전 정보 | `version.txt` | [최신 릴리즈로 이동](https://github.com/itda-skills/hyve.pub/releases/latest/download/version.txt) |

> Windows ARM64 사용자는 동일한 amd64 installer 를 다운로드하면 Windows 11 의 Microsoft Prism (x64 emulation) 으로 자동 동작합니다.

pre-release (예: `v0.1.0-rc1`) 는 위 링크에서 접근되지 않으므로 [Releases 탭](https://github.com/itda-skills/hyve.pub/releases) 에서 직접 선택하십시오.

## 설치

Windows installer (`hyve-setup-windows-amd64.exe`) 를 실행하면 다음이 구성됩니다:

- `%LOCALAPPDATA%\hyve\hyve.exe` 바이너리 설치
- 시작 메뉴 바로가기 생성 (`hyve serve` 로 MCP 서버 자동 기동)
- HKCU Run 레지스트리 등록 (로그인 시 자동 실행)
- 설치 후 `hyve serve` 자동 시작

제거는 Windows "앱 및 기능" 에서 수행하면 autostart 항목까지 함께 정리됩니다.

## 자동 업데이트

설치된 hyve 는 기동 시 본 저장소의 최신 릴리즈를 자동 확인합니다 (REST API 가 아닌 static CDN redirect 경로 사용, rate limit 비대상). 새 버전 발견 시 UI 에 알림이 표시됩니다.

## 사용 조건

본 소프트웨어는 **All Rights Reserved** 입니다. 저작권은 **쉐이크에이드** 에 있으며, 스킬.잇다 교육 과정 수강생에게 학습 목적으로 제공됩니다. 구체적인 사용 조건은 강의 자료에서 별도로 안내됩니다.

## 문의 및 이슈

문의/버그 리포트/릴리즈 asset 문제 (다운로드 실패, 체크섬 불일치 등): <dev@itda.work>

---

*이 README 는 자동 갱신되는 CI-managed 블록을 포함합니다. "최신 버전" 값은 릴리즈 시점에 github-actions\[bot\] 이 업데이트합니다.*

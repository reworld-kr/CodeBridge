# CodeBridge

> Windows용 — 폰에서 PC의 Claude Code 개발을 이어가는 릴레이 브리지.

[ReWorld](https://reworld.kr) 데스크톱 앱의 **release 배포 채널**입니다. 소스 코드는 별도 모노레포(`reworld-kr/ReWorld`)에서 관리되고, 이 repo는 빌드 산출물(`CodeBridge.exe`, NSIS installer, checksums)만 호스팅합니다.

## 다운로드

[**최신 버전 다운로드 ↓**](https://github.com/reworld-kr/CodeBridge/releases/latest)

- `CodeBridge.exe` — bare 실행 파일 (압축/설치 없이 즉시 실행)
- `CodeBridge_Setup.exe` — NSIS 설치 마법사 (사용자 디렉터리에 설치, UAC 불필요)
- `checksums.txt` — SHA-256 무결성 검증

설치 후 자동 업데이트가 켜져 있어 새 버전 출시 시 다음 실행에 백그라운드 적용됩니다.

## 주요 기능

- PC에서 돌아가는 Claude Code(또는 터미널)를 폰 브라우저에서 그대로 조작 — 외출 중에도 개발 계속
- 워크스페이스 폴더별로 '방'을 만들어 세션 분리 — 프로젝트마다 독립된 터미널
- 방 이름이 곧 접속 암호 — 폰에서 같은 이름만 입력하면 바로 연결
- relay 서버 경유라 PC에 포트 개방·공유기 설정 불필요 — NAT 뒤에서도 동작
- 여러 기기 동시 접속 — 폰·태블릿에서 같은 터미널 화면 공유
- 한글 입력 지원 + 터미널 크기 고정으로 화면 깨짐 없음
- ReWorld 계정 하나로 로그인·라이선스·자동 업데이트

## 사용법

1. 설치 후 ReWorld 계정으로 로그인합니다.
2. 개발 PC에서 CodeBridge를 켜고 '새 방'을 만듭니다 — 작업할 폴더를 고르고 비밀 방 이름을 정합니다. (이 방 이름이 폰에서 접속할 암호)
3. 방이 만들어지면 표시되는 폰 접속 주소를 폰 브라우저에서 열고, 같은 방 이름을 입력합니다.
4. PC의 Claude Code 터미널이 폰 화면에 그대로 뜹니다 — 폰에서 입력·조작하면 PC에서 실행됩니다.
5. PC는 켜둔 채 자리를 비워도 됩니다. relay는 ReWorld 공유 서버를 경유하므로 폰↔PC 직접 연결이 필요 없습니다.

## 시스템 요구사항

- Windows 10 / 11 (x64)
- 사용자 디렉터리 설치 → 관리자 권한 / UAC 불필요
- 자동 업데이트 — GitHub Release 채널 모니터링

## 라이선스

- **첫 실행 시 무료 체험** 자동 발급
- 정식 라이선스는 [reworld.kr/pricing](https://reworld.kr/pricing) 에서 구매
- 라이선스 관리 / 본인 라이선스 조회: [reworld.kr/account](https://reworld.kr/account)

데스크톱 + 모바일 + homepage 모두 **동일 ReWorld 계정**을 공유합니다.

## 문의 / 버그 리포트

- 일반 문의: [reworld.kr/contact](https://reworld.kr/contact)
- 버그 / 기능 요청: [Issues](https://github.com/reworld-kr/CodeBridge/issues)

## 관련 링크

- [CodeBridge 제품 페이지](https://reworld.kr/apps/codebridge)
- [ReWorld 앱 그리드](https://reworld.kr/apps)
- [이용약관](https://reworld.kr/legal/terms) / [개인정보처리방침](https://reworld.kr/legal/privacy)

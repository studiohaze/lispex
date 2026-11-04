# 리스펙스

[English](README.md)

리스펙스는 출판사의 표기 원칙 같은 업무 규칙을 코드로 쓰는 언어입니다. 파일과 네트워크에 손댈 수 없어서 어떤 프로그램에 넣어도 안전합니다.

이 저장소에는 리스펙스 릴리스와 공개 자료를 둡니다. 평가기 소스는 공개하지 않습니다.

[문서](https://www.lispex.com/v1.21/ko/docs/introduction) · [다운로드](https://www.lispex.com/v1.21/ko/downloads) · [플레이그라운드](https://www.lispex.com/v1.21/ko/play)

## 설치

### npm

Node.js 18 이상에서 CLI를 전역으로 설치합니다.

```sh
npm install -g lispex@1.21.2
lispex --version
```

### 네이티브

[다운로드 페이지](https://www.lispex.com/v1.21/ko/downloads)에서 리눅스, macOS, 윈도용 실행 파일을 받습니다. 각 파일의 SHA-256 체크섬도 제공합니다.

macOS와 리눅스에서는 설치 스크립트로 최신 릴리스를 받고 체크섬을 확인할 수 있습니다.

```sh
curl -fsSL https://www.lispex.com/install.sh | sh
```

윈도에서는 PowerShell에서 실행합니다.

```powershell
irm https://www.lispex.com/install.ps1 | iex
```

새 터미널에서 `lispex --version`을 실행합니다. npm과 네이티브를 함께 설치했다면 사용할 실행 파일의 경로를 `PATH`에서 먼저 둡니다.

## 언어 서버와 편집기

네이티브 실행 파일을 설치하고 `PATH`에 추가합니다. 편집기가 표준 입출력으로 언어 서버를 시작하도록 설정합니다.

```sh
lispex lsp
```

언어 서버는 문법 진단, 서식, 문서 기호, 정의 이동, 자동 완성, 내장 프로시저 설명을 제공합니다. 편집기가 보낸 문서를 대상으로 동작합니다.

[CLI 참조](https://www.lispex.com/v1.21/ko/docs/reference/cli#편집기-연결하기)에 Helix와 Neovim 설정이 있습니다. npm CLI의 `lispex lsp`는 네이티브 설치 주소를 출력하고 종료 상태 `2`를 반환합니다.

| 도구 | 지원 기능 |
| --- | --- |
| [VS Code 확장](https://github.com/studiohaze/vscode-lispex) | 구문 강조와 파일 아이콘을 제공합니다. 네이티브 1.21.2 이상에서 `lispex lsp`를 시작합니다. [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=studiohaze.lispex)와 [Open VSX](https://open-vsx.org/extension/studiohaze/lispex)에서 설치합니다. |
| [Tree-sitter](https://github.com/studiohaze/tree-sitter-lispex) | `.lspx` 파일의 문법과 편집기 쿼리를 제공합니다. |
| [highlight.js](https://github.com/studiohaze/highlightjs-lispex)와 [Prism](https://github.com/studiohaze/prism-studiohaze) | 웹페이지의 구문을 강조합니다. |
| [Pygments](https://github.com/studiohaze/pygments-topaz-lispex)와 [Rouge](https://github.com/studiohaze/rouge-studiohaze) | 문서 도구에서 구문을 강조합니다. |

## 리스펙스 배우기

[첫 프로그램](https://www.lispex.com/v1.21/ko/docs/getting-started)부터 시작해 [리스펙스 배우기](https://www.lispex.com/v1.21/ko/docs/learn)를 따라갑니다. [CLI 참조](https://www.lispex.com/v1.21/ko/docs/reference/cli)에서 터미널 명령과 편집기 설정을 확인할 수 있습니다.

## 토파즈

[토파즈](https://github.com/studiohaze/topaz)는 조판을 내장한 범용 프로그래밍 언어입니다. 문서와 다운로드는 [topaz.ooo](https://topaz.ooo)에서 제공합니다.

## 라이선스와 고지

[LICENSE](LICENSE)와 [NOTICE](NOTICE)는 공개 npm `lispex` 패키지에 포함된 파일입니다.

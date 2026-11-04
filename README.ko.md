# 리스펙스

[English](README.md)

리스펙스는 출판사의 표기 원칙 같은 업무 규칙을 코드로 쓰는 언어입니다. 파일과 네트워크에 손댈 수 없어서 어떤 프로그램에 넣어도 안전합니다.

이 저장소에서 리스펙스 릴리스를 냅니다. 평가기 소스는 이 저장소에 없습니다.

[문서](https://www.lispex.com/v1.21/ko/docs/introduction) · [다운로드](https://www.lispex.com/v1.21/ko/downloads) · [플레이그라운드](https://www.lispex.com/v1.21/ko/play)

## 설치

### npm

Node.js 18 이상이 필요합니다.

```sh
npm install -g lispex@1.21.2
lispex --version
```

### 네이티브

리눅스, macOS, 윈도용 실행 파일은 릴리스마다 첨부되고, [다운로드 페이지](https://www.lispex.com/v1.21/ko/downloads)에서도 SHA-256 체크섬과 함께 받을 수 있습니다.

macOS와 리눅스에서는 이 스크립트가 최신 릴리스를 받고 체크섬까지 확인합니다.

```sh
curl -fsSL https://www.lispex.com/install.sh | sh
```

윈도에서는 PowerShell에서 실행합니다.

```powershell
irm https://www.lispex.com/install.ps1 | iex
```

새 터미널을 열고 `lispex --version`을 실행해 보세요. npm 판과 네이티브 판을 둘 다 설치했다면 쓰려는 쪽을 `PATH` 앞에 둡니다.

## 언어 서버와 편집기

네이티브 실행 파일에는 언어 서버가 들어 있습니다. 편집기가 아래 명령을 시작하도록 설정하면 표준 입출력으로 연결됩니다.

```sh
lispex lsp
```

입력하는 동안 문법 오류를 보여 주고, 서식을 맞추고, 문서에서 정의한 이름을 모아 보여 주고, 정의로 이동하고, 내장 프로시저를 자동 완성하고 설명합니다. 편집기가 보낸 문서만 읽습니다.

Helix와 Neovim 설정은 [CLI 참조](https://www.lispex.com/v1.21/ko/docs/reference/cli#편집기-연결하기)에 있습니다. npm 판에는 언어 서버가 없어서, 거기서 `lispex lsp`를 실행하면 네이티브 다운로드 주소를 알려 주고 종료 상태 2로 끝납니다.

| 도구 | 쓸 수 있는 것 |
| --- | --- |
| [VS Code 확장](https://github.com/studiohaze/vscode-lispex) | 구문 강조와 파일 아이콘. 네이티브 리스펙스 1.21.2 이상이 있으면 `lispex lsp`도 켭니다. [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=studiohaze.lispex)나 [Open VSX](https://open-vsx.org/extension/studiohaze/lispex)에서 설치합니다. |
| [Tree-sitter](https://github.com/studiohaze/tree-sitter-lispex) | `.lspx` 파일의 문법과 편집기 쿼리. |
| [highlight.js](https://github.com/studiohaze/highlightjs-lispex)와 [Prism](https://github.com/studiohaze/prism-studiohaze) | 웹페이지 구문 강조. |
| [Pygments](https://github.com/studiohaze/pygments-topaz-lispex)와 [Rouge](https://github.com/studiohaze/rouge-studiohaze) | 문서 도구 구문 강조. |

## 리스펙스 배우기

[첫 프로그램](https://www.lispex.com/v1.21/ko/docs/getting-started)으로 시작해서 [리스펙스 배우기](https://www.lispex.com/v1.21/ko/docs/learn)로 이어 가면 됩니다. 터미널 명령과 편집기 설정은 [CLI 참조](https://www.lispex.com/v1.21/ko/docs/reference/cli)에 있습니다.

## 토파즈

[토파즈](https://github.com/studiohaze/topaz)는 조판을 내장한 범용 프로그래밍 언어입니다. 문서와 다운로드는 [topaz.ooo](https://topaz.ooo)에 있습니다.

## 라이선스

[LICENSE](LICENSE)와 [NOTICE](NOTICE)는 npm `lispex` 패키지에 들어 있는 파일과 같습니다.

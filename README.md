# Lispex

Lispex is a language for writing business rules, such as a publisher's house style. It cannot touch files or the network, so it is safe to run inside any program.

Lispex releases are published here. The evaluator source is not part of this repository.

[Documentation](https://www.lispex.com/v1.21/en/docs/introduction) · [Downloads](https://www.lispex.com/v1.21/en/downloads) · [Playground](https://www.lispex.com/v1.21/en/play)

## Install

### npm

The npm package needs Node.js 18 or later.

```sh
npm install -g lispex@1.21.2
lispex --version
```

### Native

Native executables for Linux, macOS and Windows are attached to each release and listed on the [download page](https://www.lispex.com/v1.21/en/downloads) with their SHA-256 checksums.

On macOS and Linux, this script downloads the latest release and checks its checksum.

```sh
curl -fsSL https://www.lispex.com/install.sh | sh
```

On Windows, run this in PowerShell.

```powershell
irm https://www.lispex.com/install.ps1 | iex
```

Open a new terminal and run `lispex --version`. If you have both the npm and the native version, put the one you want first on your `PATH`.

## Language server and editors

The native executable includes a language server. Set your editor to start this command, which talks over standard input and output.

```sh
lispex lsp
```

It reports syntax errors as you type, formats documents, lists the names a document defines, jumps to definitions, and completes and describes built-in procedures. It reads only the documents your editor sends.

The [CLI reference](https://www.lispex.com/v1.21/en/docs/reference/cli#connect-an-editor) has settings for Helix and Neovim. The npm version has no language server, so `lispex lsp` there points you to the native download and exits with status 2.

| Tool | What it gives you |
| --- | --- |
| [VS Code extension](https://github.com/studiohaze/vscode-lispex) | Syntax highlighting and a file icon. With native Lispex 1.21.2 or later it also starts `lispex lsp`. Install it from the [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=studiohaze.lispex) or [Open VSX](https://open-vsx.org/extension/studiohaze/lispex). |
| [Tree-sitter](https://github.com/studiohaze/tree-sitter-lispex) | A grammar and editor queries for `.lspx` files. |
| [highlight.js](https://github.com/studiohaze/highlightjs-lispex) and [Prism](https://github.com/studiohaze/prism-studiohaze) | Syntax highlighting on web pages. |
| [Pygments](https://github.com/studiohaze/pygments-topaz-lispex) and [Rouge](https://github.com/studiohaze/rouge-studiohaze) | Syntax highlighting in documentation tools. |

## Learn Lispex

Start with [First Program](https://www.lispex.com/v1.21/en/docs/getting-started) and go on to the [language lessons](https://www.lispex.com/v1.21/en/docs/learn). Terminal commands and editor setup are in the [CLI reference](https://www.lispex.com/v1.21/en/docs/reference/cli).

## Topaz

[Topaz](https://github.com/studiohaze/topaz) is a general-purpose programming language with typesetting built in. Its documentation and downloads are at [topaz.ooo](https://topaz.ooo).

## License

[LICENSE](LICENSE) and [NOTICE](NOTICE) are the same files that ship in the `lispex` npm package.

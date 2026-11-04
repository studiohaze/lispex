# Lispex

[한국어](README.ko.md)

Lispex is a language for writing business rules, such as a publisher's house style. It cannot touch files or the network, so it is safe to run inside any program.

This repository holds Lispex releases and public material. The evaluator source is not published.

[Documentation](https://www.lispex.com/v1.21/en/docs/introduction) · [Downloads](https://www.lispex.com/v1.21/en/downloads) · [Playground](https://www.lispex.com/v1.21/en/play)

## Install

### npm

With Node.js 18 or newer, install the CLI globally.

```sh
npm install -g lispex@1.21.2
lispex --version
```

### Native

Download the executable for Linux, macOS, or Windows from the [download page](https://www.lispex.com/v1.21/en/downloads). It includes a SHA-256 checksum for each file.

For macOS and Linux, the installer downloads the current release and checks its checksum.

```sh
curl -fsSL https://www.lispex.com/install.sh | sh
```

For Windows, run this in PowerShell.

```powershell
irm https://www.lispex.com/install.ps1 | iex
```

Open a new terminal and run `lispex --version`. If you install both npm and Native, put the executable you want first on `PATH`.

## Language server and editors

Install the native executable and put it on `PATH`. Configure your editor to start the language server over standard input and output.

```sh
lispex lsp
```

The server provides syntax diagnostics, formatting, document symbols, go to definition, completion, and built-in procedure descriptions. It works on documents sent by the editor.

The [CLI reference](https://www.lispex.com/v1.21/en/docs/reference/cli#connect-an-editor) includes Helix and Neovim settings. In the npm CLI, `lispex lsp` prints the native installation address and exits with status `2`.

| Tool | Support |
| --- | --- |
| [VS Code extension](https://github.com/studiohaze/vscode-lispex) | Syntax highlighting and a file icon. Starts `lispex lsp` with Native 1.21.2 or later. Available on [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=studiohaze.lispex) and [Open VSX](https://open-vsx.org/extension/studiohaze/lispex). |
| [Tree-sitter](https://github.com/studiohaze/tree-sitter-lispex) | Grammar and editor queries for `.lspx` files. |
| [highlight.js](https://github.com/studiohaze/highlightjs-lispex) and [Prism](https://github.com/studiohaze/prism-studiohaze) | Syntax highlighting for web pages. |
| [Pygments](https://github.com/studiohaze/pygments-topaz-lispex) and [Rouge](https://github.com/studiohaze/rouge-studiohaze) | Syntax highlighting for documentation tools. |

## Learn Lispex

Start with [First Program](https://www.lispex.com/v1.21/en/docs/getting-started), then follow the [language lessons](https://www.lispex.com/v1.21/en/docs/learn). The [CLI reference](https://www.lispex.com/v1.21/en/docs/reference/cli) covers terminal commands and editor setup.

## Topaz

[Topaz](https://github.com/studiohaze/topaz) is a general-purpose programming language with typesetting built in. Visit [topaz.ooo](https://topaz.ooo) for its documentation and downloads.

## License and notices

[LICENSE](LICENSE) and [NOTICE](NOTICE) are the files shipped with the public `lispex` npm package.

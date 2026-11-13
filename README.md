# Lispex

Lispex is a language for business rules, such as a publisher's house style or a shipping fee. A rule gives the same answer for the same input, and it cannot touch files or the network, so it is safe to run inside any program.

[Website](https://www.lispex.com) · [Playground](https://www.lispex.com/v1.21/en/play) · [Roadmap](https://www.lispex.com/v2.0/en/docs/project/roadmap) · [Download 1.21.3](https://www.lispex.com/v1.21/en/downloads) · [Topaz](https://github.com/studiohaze/topaz)

## Two lines of Lispex

| Version | Status | What it is |
| --- | --- | --- |
| 1.21.3 | **Stable** | The release you can install and use today. Its releases are published here. |
| 2.0 | **Spec-first redesign** | A specification written first and an evaluator that follows it. It runs inside Topaz 6 and is validated in ATLAS together with Topaz 6. |

## Where 2.0 is going

Lispex 2 starts from the specification. The evaluator follows it, and every change is checked against it. The [roadmap](https://www.lispex.com/v2.0/en/docs/project/roadmap) shows the required checks that pass at each stage and the known limitations that remain, generated from those checks.

Lispex 2 runs inside Topaz 6 as its sandboxed rule module. A Topaz program hands a rule its input and limits, and the rule can use only what the host gives it. ATLAS, the flagship program of STUDIO HAZE, validates Topaz 6 before its public release, and Lispex 2 goes through ATLAS with it. Lispex 2 itself ships once every stage of its specification passes, without waiting for Topaz 6.

Alongside Topaz 6.0, the public parts of Lispex move to this repository. That covers the language specification, the embedding contract Topaz uses and a conformance suite, so anyone can check the safety promise for themselves.

## Use Lispex 1.21.3 today

```sh
npm install -g lispex@1.21.3          # Node.js 18 or later
curl -fsSL https://www.lispex.com/install.sh | sh    # native, macOS and Linux
```

On Windows, run `irm https://www.lispex.com/install.ps1 | iex` in PowerShell. Native executables for every platform and their SHA-256 checksums are on the [download page](https://www.lispex.com/v1.21/en/downloads).

Start with [First Program](https://www.lispex.com/v1.21/en/docs/getting-started). The native executable includes a language server (`lispex lsp`), and the [CLI reference](https://www.lispex.com/v1.21/en/docs/reference/cli#connect-an-editor) shows how to connect an editor. Syntax highlighting is available for [VS Code](https://github.com/studiohaze/vscode-lispex), [Tree-sitter](https://github.com/studiohaze/tree-sitter-lispex), [highlight.js](https://github.com/studiohaze/highlightjs-lispex), [Prism](https://github.com/studiohaze/prism-studiohaze), [Pygments](https://github.com/studiohaze/pygments-topaz-lispex) and [Rouge](https://github.com/studiohaze/rouge-studiohaze).

## License

Lispex is released under the [Apache License 2.0](LICENSE), for both the npm package and the native executables. See [NOTICE](NOTICE). Each release also includes `THIRD-PARTY-NOTICES.txt` with the licenses of the libraries built into the executables. The evaluator source is not part of this repository.

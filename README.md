# Monokai Dark Soda ZJY

A personal fork of [Monokai Dark Soda](https://github.com/AdamCaviness/vs-code-theme-monokai-dark-soda) by [AdamCaviness](https://github.com/AdamCaviness), with UI and syntax tweaks for daily use in VS Code and Cursor.

> This theme traces back to the excellent [Monokai Dark Soda TextMate theme](https://github.com/mrlundis/Monokai-Dark-Soda.tmTheme) by mrlundis.

![](theme-monokai-dark-soda.png)

## Fork Information

| | Upstream | This fork |
|---|---|---|
| **Extension ID** | `AdamCaviness.theme-monokai-dark-soda` | `zjy.theme-monokai-dark-soda-zjy` |
| **Theme label** | Monokai Dark Soda | Monokai Dark Soda ZJY |
| **Repository** | [AdamCaviness/vs-code-theme-monokai-dark-soda](https://github.com/AdamCaviness/vs-code-theme-monokai-dark-soda) | [ZhangJYd/vs-code-theme-monokai-dark-soda-zjy](https://github.com/ZhangJYd/vs-code-theme-monokai-dark-soda-zjy) |
| **Publisher** | AdamCaviness | zjy |

### Changes in this fork

- Brighter sidebar and terminal text
- VS Code-style blue selection and accent colors
- Softer, more visible word-occurrence highlighting
- Classic Monokai purple (`#AE81FF`) for constants across LSP-supported languages
- Semantic token rules for `readonly`, `enumMember`, and static constants (Go, Python, TypeScript, Rust, Java, C#, etc.)

## Installation

### Cursor / VS Code (Open VSX)

Search for **Monokai Dark Soda ZJY** in the Extensions panel, or install from [Open VSX](https://open-vsx.org) after publishing.

### Manual install (.vsix)

```bash
# Build
npx @vscode/vsce package --allow-missing-repository

# Cursor
cursor --install-extension theme-monokai-dark-soda-zjy-<version>.vsix

# VS Code
code --install-extension theme-monokai-dark-soda-zjy-<version>.vsix
```

### Set as default theme

```json
{
  "workbench.colorTheme": "Monokai Dark Soda ZJY"
}
```

### LSP constant highlighting

This theme colors constants via **semantic tokens** (LSP) and **TextMate scopes** (fallback). Installing the extension enables semantic highlighting by default.

| Language | LSP / Extension | What's highlighted |
|----------|-----------------|-------------------|
| Go | gopls | `const`, enum members |
| Python | Pylance | `UPPER_CASE` constants, class constants |
| TypeScript / JavaScript | built-in TS server | `const`, `readonly`, enum members |
| Rust | rust-analyzer | `const`, enum variants |
| Java / C# | Red Hat Java / C# Dev Kit | `static final` / `const` fields, enum members |
| Others | any LSP with semantic tokens | tokens marked `readonly` or `enumMember` |

Requires a language extension with semantic highlighting support. If constants are not purple, check that semantic highlighting is enabled:

```json
{
  "editor.semanticHighlighting.enabled": true
}
```

Go-specific (also enabled by this theme's defaults):

```json
{
  "gopls": {
    "ui.semanticTokens": true
  }
}
```

## Color Palette

Palette      | Hex       | Notes
---          | ---       | ---
Background   | `#242424` |
Current Line | `#3D3D3D` |
Selection    | `#264f78` | VS Code-style blue (fork change)
Comment      | `#8C8C8C` |
Foreground   | `#F8F8F2` |
String       | `#FFEE99` |
Constant     | `#AE81FF` | Classic Monokai purple (fork change)
Keyword      | `#F92672` |
Function     | `#A6E22E` |
Type         | `#66D9EF` |

## Upstream

If you prefer the original theme without these customizations, install the upstream extension:

```sh
ext install AdamCaviness.theme-monokai-dark-soda
```

Please report issues with **this fork** in [this repository](https://github.com/ZhangJYd/vs-code-theme-monokai-dark-soda-zjy/issues). For the original theme, use [AdamCaviness/vs-code-theme-monokai-dark-soda](https://github.com/AdamCaviness/vs-code-theme-monokai-dark-soda/issues).

## License

This fork is distributed under the [MIT License](LICENSE). Copyright (c) 2019 Adam Caviness. Modifications in this fork are also released under the MIT License.

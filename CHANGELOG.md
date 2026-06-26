# Change Log

All notable changes to **Monokai Dark Soda ZJY** (this fork) are documented here.
Upstream history for the original theme is preserved below.

## 1.2.3 - 2026-06-25 (ZJY fork)

- Tuned workbench and terminal text selection colors for rename inputs, chat, and terminal
- New extension icon (`theme-monokai-dark-soda-zjy.png`) using the theme palette
- README preview screenshot updated

## 1.2.2 - 2026-06-25 (ZJY fork)

- Selection and list focus colors changed from VS Code blue to semi-transparent gray-white
- Softer peek/reference match highlights (`peekViewEditor`, `peekViewResult`)
- Visible unfocused input borders for chat and panel inputs (`input`, `panelInput`, `agentsChatInput`)
- Unified panel and dropdown border colors; minimap and peek result selection aligned with new selection palette
- Improved inactive (unfocused window) selection visibility

## 1.2.1 - 2026-06-23 (ZJY fork)

Fork of [AdamCaviness/vs-code-theme-monokai-dark-soda](https://github.com/AdamCaviness/vs-code-theme-monokai-dark-soda) v1.2.0.

- Brighter sidebar, file tree, and terminal foreground colors
- VS Code-style blue selection and list focus colors
- Improved word-occurrence highlighting with softer light-blue borders
- Constants use classic Monokai purple (`#AE81FF`) instead of `#FF80F4`
- Go `const` and enum member highlighting via TextMate scopes and semantic tokens
- Published as `zjy.theme-monokai-dark-soda-zjy`

---

## Upstream: Monokai Dark Soda

## 1.2.0 - 2023-04-04
- Reverted to original colors based on feedback!

## 1.1.0 - 2023-04-04
- Added ChangeLog
- Italics are now used for comments. @iVenomWeed.
- Added comment punctuation definition. @iVenomWeed.
- Added many new scopes for several languages (not semantic support yet). If you see a disruptive change, please open an issue and I'll fix it.
    - C#
    - C++
    - JSON
    - Java
    - JavaScript
    - TypeScript
    - Elixir
    - CSS
    - Markdown
    - Latex
    - Python
    - Rust

## 1.0.0 - 2021-01-12
- Added Code of Conduct. @MadhanDevlpr
- Migrated from tmTheme to json.
- Fixed non-workbench foreground and highlight colors. @godrix

## 0.0.6 - 2019-12-16
- Added settings JS string interpolation expression. @godrix
- LineHighlight hexadecimal correction. @godrix

## 0.0.5 - 2015-12-21
- initial release
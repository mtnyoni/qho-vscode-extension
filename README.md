# Ndebele Language — VS Code Extension

Syntax highlighting for `.ndb` files written in the Ndebele programming language.

## Features

- Keywords highlighted by category:
    - **Control flow**: `uma`, `phindaUma`, `phinda`, `phuma`, `qhubeka`, `phendukisa`, `kungela`
    - **Types**: `inombolo`, `ibala`
    - **Declarations**: `isigoqelo`, `isakhi`, `bumba`, `yenza`
    - **Built-ins**: `bhala`, `mina`
- String literals, number literals, `akulalutho` (nil)
- Function calls, method calls, struct names
- Line comments (`//`)
- Bracket matching and auto-closing pairs

## Installation

### Option A — Install from `.vsix` (recommended for local dev)

1. Install dependencies and package:
    ```bash
    npm install
    npx vsce package
    ```
2. This produces `qho-0.1.0.vsix`.
3. In VS Code: `Ctrl+Shift+P` → **Extensions: Install from VSIX...** → select the file.

### Option B — Sideload during development

1. Copy this folder to your VS Code extensions directory:
    - **Linux/macOS**: `~/.vscode/extensions/qho`
    - **Windows**: `%USERPROFILE%\.vscode\extensions\qho`
2. Restart VS Code.

### Option C — Open in VS Code and press F5

Open this folder in VS Code, then press **F5** to launch an Extension Development Host with the grammar active.

## Usage

Open or create any file with a `.ndb` extension and the highlighting activates automatically.

## File Extension

`.ndebele` .

## Keyword Reference

| Ndebele      | Meaning             |
| ------------ | ------------------- |
| `bhala`      | print               |
| `inombolo`   | float64 type        |
| `ibala`      | string type         |
| `uma`        | if                  |
| `phindaUma`  | while               |
| `phinda`     | loop (infinite)     |
| `phuma`      | break               |
| `qhubeka`    | continue            |
| `isigoqelo`  | function            |
| `isakhi`     | struct              |
| `bumba`      | instantiate struct  |
| `yenza`      | val (binding)       |
| `phendukisa` | return              |
| `mina`       | self                |
| `akulalutho` | nil                 |
| `kungela`    | syntactic nil check |

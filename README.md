# zoxide-plus

Single-file installer for the `j` directory-jump command.

- 中文说明：[`README.zh-CN.md`](./README.zh-CN.md)

## Install

```bash
curl -fsSL <YOUR_INSTALL_URL> | zsh
```

The installer will automatically:
- check and install `zoxide`
- create `~/.zoxide-plus/zoxide-plus` locally
- append `source ~/.zoxide-plus/zoxide-plus` to `~/.zshrc`

Then reload your shell:

```bash
source ~/.zshrc
```

## Usage

### 1. Jump by keyword

```bash
j wx
```

If only one directory matches, it jumps directly.

If multiple directories match, the terminal shows a numbered list and asks you to choose one.

### 2. Fallback to Finder picker

```bash
j something-new
```

If no history entry matches, a Finder-style folder picker opens. After selection, the shell jumps into that directory.

### 3. No keyword

```bash
j
```

This opens the Finder folder picker directly.

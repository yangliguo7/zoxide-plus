# zoxide-plus 中文说明

`zoxide-plus` 是一个单文件安装器，用来提供增强版目录跳转命令 `j`。

- English guide: [`README.md`](./README.md)

## 一键安装

```bash
curl -fsSL https://raw.githubusercontent.com/yangliguo7/zoxide-plus/main/install-zoxide-plus | zsh
```

安装脚本会自动完成：
- 检查并安装 `zoxide`
- 在本地生成 `~/.zoxide-plus/zoxide-plus`
- 把 `source ~/.zoxide-plus/zoxide-plus` 写入 `~/.zshrc`

然后执行：

```bash
source ~/.zshrc
```

## 使用方法

### 1. 按关键词跳转

```bash
j wx
```

如果只匹配到一个目录，会直接跳转。

如果匹配到多个目录，终端会显示候选列表，并让你输入序号选择。

### 2. 无匹配时手动选择目录

```bash
j something-new
```

如果没有匹配到历史目录，会弹出 Finder 目录选择框，选择后自动跳转。

### 3. 不传关键词

```bash
j
```

会直接弹出 Finder 目录选择框。

# opencli-platform-router

这个 skill 依赖本机 `opencli` 命令和 Chrome 扩展。

## 安装前置

### 1) 安装 opencli CLI

```bash
npm install -g @jackwener/opencli
opencli --version
```

### 2) 手动安装 Chrome 扩展（必需）

> 当前需要手动安装 Browser Bridge 扩展，安装后才能复用 Chrome 登录态。

两种方式任选其一：

- 方式 A（推荐）：从项目 Release 下载 `opencli-extension.zip`
- 方式 B（开发态）：打开 `chrome://extensions` → 开启开发者模式 → Load unpacked → 选择 opencli 仓库里的 `extension/` 目录

安装后保持 Chrome 打开，并确保你已经登录目标平台账号。

### 3) 连接自检

```bash
opencli doctor
```

## 用法

1. 进入 `skills/opencli-platform-router/references/commands/`
2. 按平台查找文档（如 `twitter.md`、`xiaohongshu.md`）
3. 按文档给出的命令和参数执行

常用格式：

```bash
opencli <site> <command> [--args] -f json
```

示例：

```bash
opencli twitter search --query "ai agent" --limit 20 -f json
opencli zhihu hot --limit 20 -f json
opencli bilibili search --keyword "大模型" --limit 20 -f json
```

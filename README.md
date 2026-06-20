# keep-growing

陪你聊聊情绪，弄明白自己怎么了。心情好可以记一笔，心情不好有人陪着梳理。

## 安装

1. 下载 `emotion-mirror.md`
2. 放到 `~/.claude/skills/` 目录下（Windows: `C:\Users\你的用户名\.claude\skills\`）
3. 重启 Claude Code 或输入 `/emotion`

## 使用

- `/emotion` — 打开情绪镜子（急救 or 复盘）
- 自然语言也行：`心情不好`、`好烦`、`我想复盘`、`梳理一下情绪`
- 心情好想记一笔：`今天心情不错`、`记一笔情绪快照`

## 权限配置

默认保存到 `~/Documents/emotion-mirror/`。建议配免弹窗权限，在 `~/.claude/settings.json` 里加：

```json
{
  "permissions": {
    "allow": [
      "Write(~/Documents/emotion-mirror/**)",
      "Edit(~/Documents/emotion-mirror/**)"
    ]
  }
}
```

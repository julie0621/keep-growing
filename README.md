# keep-growing

> 作者：julie0621 · 仓库：[github.com/julie0621/keep-growing](https://github.com/julie0621/keep-growing)

情绪复盘 · 工具监测。一个陪你看内在，一个帮你看外面。

---

## 🪞 Emotion Mirror 情绪镜子

陪你聊聊情绪，弄明白自己怎么了。心情好可以记一笔，心情不好有人陪着梳理。不诊断、不替你做决定。

- `/emotion` — 打开情绪镜子（急救 or 复盘）
- 自然语言也可触发：`心情不好`、`好烦`、`我想复盘`、`今天挺开心`……

---

## 🔧 Angry Migrator 工具健康度体检

SaaS 工具健康度体检——监控评分趋势、定价变动与条款暗坑，寻找替代方案。看准数据再决定，不冲动也不拖延。

- `/angry` — 打开工具体检（体检 or 替代品 or 监控列表 or 工具动向）
- 自然语言也可触发：`帮我查一下这个工具`、`有什么替代`、`加入监控`……

---

## 安装

### 方式一：插件市场（推荐）

在 Claude Code 中输入：

```
/plugin marketplace add julie0621/keep-growing
/plugin install emotion-mirror
/plugin install angry-migrator
```

### 方式二：手动安装

1. 下载 `emotion-mirror.md` / `angry-migrator.md`
2. 放到 `~/.claude/skills/` 目录下（Windows: `C:\Users\你的用户名\.claude\skills\`）
3. 重启 Claude Code 即可使用

---

## 权限配置（建议但不必须）

Skill 保存记录或写入文件时，默认每次都会弹权限确认框。配一下就能静默通过。

打开或新建 `~/.claude/settings.json`（Windows: `C:\Users\你的用户名\.claude\settings.json`），加入：

```json
{
  "permissions": {
    "allow": [
      "Write(~/Documents/emotion-mirror/**)",
      "Edit(~/Documents/emotion-mirror/**)",
      "Write(~/Documents/angry-migrator/**)",
      "Edit(~/Documents/angry-migrator/**)"
    ]
  }
}
```

重启 Claude Code 生效。不用做别的。

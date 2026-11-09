# 英语单词听写

一款可离线使用的英语单词听写 PWA。浏览器语音朗读单词，支持美音 / 英音、自定义词库、听写判分与错词重练。

## 在线使用

https://english-2026user.github.io/word-dictation/

## 安装到桌面

- **Android（Chrome）**：打开网址 → 菜单 → 安装应用 / 添加到主屏幕
- **iPhone（Safari）**：打开网址 → 分享 → 添加到主屏幕

首次联网打开会缓存全部资源，之后断网也能使用。

## 本地运行

```bash
cd word-dictation
python3 -m http.server 8000
```

浏览器打开 http://localhost:8000

## 部署

- **GitHub Pages**：仓库 Settings → Pages → Source 选 `main` 分支根目录 → Save
- **Vercel**：`npx vercel --prod`（已含 `vercel.json` 配置）

## 文件说明

| 文件 | 说明 |
| --- | --- |
| `index.html` | 应用主体（含全部功能逻辑） |
| `manifest.json` | PWA 配置（应用名、图标、显示模式） |
| `sw.js` | Service Worker 离线缓存 |
| `icons/` | 应用图标（192 / 512 / 掩码 / Apple 触控） |
| `vercel.json` | Vercel 部署与缓存头配置 |

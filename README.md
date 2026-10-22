# 网盘搜索器

单文件网页版网盘搜索器，支持安装为 PWA。

- 电脑：左侧选择站点，右侧直接预览搜索结果。
- 手机：浏览器打开后「添加到主屏幕」，像 App 一样全屏使用。

## 文件

- `index.html` — 页面本体（所有逻辑和站点数据都在里面）
- `manifest.webmanifest` — PWA 配置
- `sw.js` — Service Worker，缓存页面外壳供离线打开
- `icons/` — 应用图标

## 更新

修改 `index.html` 后提交并推送，GitHub Pages 会自动发布。Service Worker 对页面采用网络优先策略，刷新即可拿到新版本。

## 部署

仓库 Settings → Pages → Source 选择 `Deploy from a branch`，分支 `main`，目录 `/`。

# stillfloating-workspace

[Still Floating](https://stillfloating.top) 的私人工作区（`/workspace/`）源码：以「土星舱室」为视觉主题的个人服务导航、实时配额看板与 Codeforces 刷题状态面板。

## 主要文件

- `index.php`：工作区主入口与舱室卡片配置（`CORE` / `FILE` / `NOTE` / `FEED` / `WATCH` / `REMOTE`），支持口令页与 `?k=<token>` Cookie 会话鉴权。
- `lib.php`：页面骨架渲染、公共鉴权与辅助函数。
- `ws.css` / `ws.js`：土星星图视觉样式、交互筛选（`⌘K`）、实时状态刷新逻辑。
- `bay.svg` / `map.svg`：舱室与星图矢量图形资源。
- `quota.php` / `cf.php` / `status.php`：后端模型配额、Codeforces 提交状态与站点健康接口。

## 本地预览

安装 PHP CLI 后，可以导出一份静态预览：

```bash
SF_WS_PREVIEW=1 php index.php > preview.html
```

预览文件和样式、脚本、图形资源放在同一目录。接入实时接口前，需配置自己的私有授权文件和后端服务。

## 2026-11-18 公开版更新

将服务链接、账号和后端配置路径改为示例值，保留页面、鉴权逻辑与状态接口供参考。 [查看更新提交](https://github.com/zts8989898937-coder/stillfloating-workspace/commit/462293f7f8fef3ead196bf80fe9bb7b606cc4437)

[公开范围](PUBLIC_SCOPE.md) · [架构说明](docs/ARCHITECTURE.md) · [后续路线](docs/ROADMAP.md)

# stillfloating-workspace

[Still Floating](https://stillfloating.top) 的私人工作区（`/workspace/`）源码：以「土星舱室」为视觉主题的个人服务导航、实时配额看板与 Codeforces 刷题状态面板。

## 主要文件

- `index.php`：工作区主入口与舱室卡片配置（`CORE` / `FILE` / `NOTE` / `FEED` / `WATCH` / `REMOTE`），支持口令页与 `?k=<token>` Cookie 会话鉴权。
- `lib.php`：页面骨架渲染、公共鉴权与辅助函数。
- `ws.css` / `ws.js`：土星星图视觉样式、交互筛选（`⌘K`）、实时状态刷新逻辑。
- `bay.svg` / `map.svg`：舱室与星图矢量图形资源。
- `quota.php` / `cf.php` / `status.php`：后端模型配额、Codeforces 提交状态与站点健康接口。

## 公开版本说明

部署参数使用示例值。公开范围见 [PUBLIC_SCOPE.md](PUBLIC_SCOPE.md)，通用框架和路线见 [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) 与 [docs/ROADMAP.md](docs/ROADMAP.md)。

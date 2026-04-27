# 项目说明

Kodi 插件 `plugin.video.filteredmovies` — 电影剧集筛选和增强工具。

## 开发调试

- kodi JSON-RPC 测试地址: `127.0.0.1:8080/jsonrpc`
- Kodi 源码位于 workspace 中的 `xbmc` 文件夹
- JSON-RPC API 文档: https://kodi.wiki/view/JSON-RPC_API/v13

## 项目结构

- `default.py` — 插件入口，路由分发到各功能
- `service.py` — 后台服务（片头片尾自动跳过、播放列表自动补全、遮罩修复等）
- `lib/common.py` — 公共工具函数
- `lib/video_library.py` — 视频库 JSON-RPC 查询
- `lib/media_info.py` — 字幕/音轨信息获取
- `lib/window_handler.py` — 自定义窗口管理
- `lib/t9_helper.py` — T9 拼音搜索
- `resources/skins/` — UI 皮肤 XML 文件
- `dev/` — 开发辅助脚本

## 注意事项

- 如果需求有不明确的地方，停下来等待用户补充确认
- 禁止使用 PowerShell 进行文本替换

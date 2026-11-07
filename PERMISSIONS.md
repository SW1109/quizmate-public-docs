---
title: 权限与数据流
permalink: /permissions/
---

# 浏览器权限与数据流

对应版本：0.8.0。更新日期：2026 年 11 月 7 日。

## 权限用途

| 权限 | 当前用途 |
| --- | --- |
| `activeTab` | 用户主动操作时访问当前标签页的必要上下文。 |
| `scripting` | 在已授权页面注入包内的识题、受控填写及页内控件脚本。 |
| `storage` | 保存设置、同意记录、授权会话、会话记录和可选加密凭据。 |
| `sidePanel` | 展示运行状态、日志筛选和搜索；完整工作台与设置在独立标签页。 |
| `nativeMessaging` | 本地 CLI 模式与另行安装的本地桥通信；官方及 API 模式不依赖该桥。 |
| `webNavigation` | 识别已授权练习页面及 iframe 导航，保持题目绑定。 |
| `offscreen` | 在侧栏收起时维持可取消的 API 请求处理。 |
| 有限 `host_permissions` | 支持下列课程站点的识别，以及用户启动后的正常播放和练习操作。 |
| `optional_host_permissions` | 允许用户按需授权特定练习站点、授权后台或 API 域名；声明的 HTTP/HTTPS 范围是可选授权池。 |

## 预置课程站点

- `https://*.chaoxing.com/*`
- `https://*.zhihuishu.com/*`
- `https://www.icourse163.org/*`
- `https://moodle.syxy.ouchn.cn/*`

安装并不默认授权全部网站。其他练习页和接口域名按需申请；可在浏览器扩展管理页限制或移除权限。扩展未声明 `cookies`、`history`、`webRequest`、`debugger` 或 `management` 权限。供页面展示的可访问资源仅为静态图标。

## 数据去向

官方-题库+ AI Nexly 模式把必要题目内容发送给授权后台，先匹配题库，未可靠命中时调用后台配置的模型服务；调用与计费记录保留于后台。自配 API 将题目直接发送给所配置接口；本地 CLI 交由本机工具处理。后两种模式会另行向授权后台核验时长，不把题目或模型凭据附加到核验请求。

课程目录、视频、文档正文不会作为模型请求上传。后台管理员主动查询 IP 地区时，相关 IP 会发送至地区查询服务。具体数据类型、保留及清理方式见[隐私政策](https://sw1109.github.io/quizmate-public-docs/privacy/)。

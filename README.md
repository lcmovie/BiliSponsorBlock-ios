# BiliSponsorBlock-ios

适用于官方哔哩哔哩 iOS App 的空降助手插件，通过注入 dylib 的方式提供 SponsorBlock 片段识别、提示和自动跳过功能。

## 可实现的功能

- 自动识别当前视频的 BV 号和 CID
- 获取并解析 SponsorBlock 空降片段
- 自动跳过赞助、自我推广、互动提醒、片头片尾、离题等分类片段
- 为不同片段分类设置独立处理方式
- 支持“总是跳过”“跳过一次”“手动跳过”“仅显示”和“禁用”
- 使用中文显示片段分类和跳过提示
- 在播放器进度条上以分类颜色标记片段位置
- 拖动或展开原生进度条时，彩色片段标记同步移动
- 视频、分P或播放会话切换时清理旧片段，避免跨视频复用
- 支持从首页、动态、搜索、UP主页和相关推荐进入视频
- 在哔哩哔哩设置页面中提供独立的“空降助手”设置入口
- 记录跳过次数和累计节省时间
- 支持总开关和插件功能配置
- 支持指定UP主关注状态验证，并可跳转到哔哩哔哩App内个人空间

本插件借助 [BilibiliSponsorBlock](https://github.com/hanydd/BilibiliSponsorBlock) 项目的支持，实现空降片段数据获取与相关功能。

## 功能预览

<table>
  <tr>
    <td width="50%"><img src="docs/images/preview-1.jpg" alt="设置页面入口" width="100%"></td>
    <td width="50%"><img src="docs/images/preview-2.jpg" alt="空降助手设置" width="100%"></td>
  </tr>
  <tr>
    <td width="50%"><img src="docs/images/preview-3.jpg" alt="自动跳过与彩色进度条" width="100%"></td>
    <td width="50%"><img src="docs/images/preview-4.jpg" alt="横屏播放效果" width="100%"></td>
  </tr>
</table>

## 当前适配范围

- iOS 15.0 及以上
- ARM64
- 官方哔哩哔哩 iOS App 9.0.0
- 可用于支持 dylib 注入的安装方式

不同哔哩哔哩版本的播放器结构和内部接口可能发生变化，因此其他版本需要单独验证和适配。

## 说明

本仓库用于介绍项目功能，暂不公开插件源码。项目仅供学习、研究和个人使用，请遵守相关平台规则及所在地法律法规。

SponsorBlock 片段数据由相应服务提供，片段准确性取决于社区提交内容。

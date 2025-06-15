简介
TuDouKit（土豆浏览器） 是基于 Chromium 引擎开发的高匿名度指纹浏览器，兼容 Windows 7 及以上操作系统，未来还将支持 macOS、Android、Linux 等多种平台。

浏览器指纹识别 是通过收集用户的浏览器、操作系统和硬件特征（如 User-Agent、语言、屏幕分辨率、字体、插件、时区、WebGL 等）生成的唯一识别码。网站或第三方可以利用这一机制来追踪用户行为、分析身份、实施广告定向，甚至进行钓鱼或欺诈。

为了保护隐私、进行广告防追踪、自动化测试或跨境营销，土豆浏览器（TuDouKit） 提供了比原生 Chromium 更强的匿名性和多环境管理能力。

TuDouKit（土豆浏览器）核心优势
相较于原始的 Chromium 浏览器，TuDouKit 拥有以下两大核心优势：

✅ 支持在一台设备上创建多个浏览器指纹环境，可模拟多个独立用户。

✅ 支持多浏览器环境的统一管理，便于账号批量运营、广告投放测试、自动化脚本运行等场景。

快速开始
1. 下载与安装
前往 TuDouKit 官方网站 或其 GitHub 发布页 下载最新版安装包，适用于 Windows 7 及以上系统。

2. 创建新的浏览器环境
打开 土豆浏览器 TuDouKit 应用，点击“创建浏览器”。
在弹出的配置窗口中，你可以自定义指纹参数，或者选择使用默认推荐配置。

3. 启动指纹浏览器
点击“启动”按钮，即可打开独立指纹环境的浏览器实例。

支持的浏览器指纹修改项（亲测有效）
可通过 fingerprintjs 和 browserleaks 等网站测试指纹变更效果。TuDouKit 支持以下指纹项目自定义或伪装：

类别	可修改内容
系统信息	操作系统（User-Agent 中显示）、CPU 核心数、内存、设备名称、MAC 地址等
浏览器参数	浏览器版本、User-Agent、自定义代理（支持默认/不使用/自定义代理）
语言与时区	navigator.language、navigator.languages、new Date() 时区，可基于 IP 匹配
Web相关API	WebRTC（本地 IP 遮蔽）、Geolocation 经纬度模拟、Canvas 和 WebGL 伪装像素图、AudioContext 音频指纹扰动、Speech Voices 等
显示设置	屏幕分辨率（screen.width/screen.height）、字体（支持字体列表随机化）
其他特征	ClientRects、Do Not Track 状态、SSL 签名信息、端口扫描保护、硬件加速控制、自动化防检测（如 navigator.webdriver=false）等

自动化控制支持
TuDouKit 完全基于 Chromium 构建，可兼容自动化测试框架，如：

Playwright

Puppeteer

我们也提供了官方自动化脚本示例，详见：GitHub Automation Demo。

参与和支持 TuDouKit
TuDouKit（土豆浏览器） 仍在积极开发中，欢迎加入我们：

⭐ 贡献代码或提交 Issue，帮助修复 Bug 与添加新功能。

🧪 试用 TuDouKit 浏览器并反馈问题，尤其是在不同网站上的兼容性与指纹绕过效果。

💬 分享你的使用经验，通过博客、论坛或社交平台帮助推广 TuDouKit。

🌐 加入开发者社区，参与讨论，获得技术支持与最新进展。

免责声明
本项目仅用于技术研究与学习用途，禁止用于任何非法目的。任何因使用本项目导致的损失（包括但不限于数据丢失、法律责任等），作者概不负责。

您在使用 TuDouKit 时必须明确承诺不会将其用于违法行为，包括但不限于侵犯隐私、欺诈、钓鱼、攻击网站等。


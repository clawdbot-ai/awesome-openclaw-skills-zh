# Awesome Moltbot Skills (中文官方库)
> 翻译自 [Clawdbot 官方技能库](https://clawdhub.com/skills)，持续同步更新。
> 所有技能已适配中文指令，可直接在 Moltbot 中调用（支持 Telegram/企业微信/本地客户端）。


## 一、办公自动化 📊
| 英文技能名 | 中文技能名 | 官方技能链接 | 核心功能（中文翻译） | 中文调用示例 |
|-----------|-----------|------------|----------------------|--------------|
| Email Sender | 邮件自动发送 | [Clawdbot/email-sender](https://clawdhub.com/skills/email-sender) | 支持批量发送邮件、附件上传、模板化正文，可定时发送 | 「给张三、李四发邮件，主题是“周报汇总”，附件是D盘的“周报.xlsx”，正文用模板1」 |
| Calendar Sync | 日历同步助手 | [Clawdbot/calendar-sync](https://clawdhub.com/skills/calendar-sync) | 同步谷歌/Outlook/企业微信日历，自动创建会议、发送提醒 | 「把明天下午3点的客户会议同步到企业微信日历，提醒参会人提前10分钟」 |
| Document Scanner | 文档扫描识别 | [Clawdbot/document-scanner](https://clawdhub.com/skills/document-scanner) | 拍摄图片/上传文件，自动OCR识别文字、转为PDF/Word | 「把这张纸质报表扫描成PDF，提取文字内容保存到桌面」 |
| Excel Processor | Excel 自动化处理 | [Clawdbot/excel-processor](https://clawdhub.com/skills/excel-processor) | 数据清洗、格式转换、公式计算、报表生成，支持批量操作 | 「把文件夹里所有Excel的“销售额”列求和，生成汇总表保存到D盘」 |
| Meeting Notes Generator | 会议纪要生成器 | [Clawdbot/meeting-notes-generator](https://clawdhub.com/skills/meeting-notes-generator) | 录制会议音频/导入转录文本，自动提取关键点、生成结构化纪要 | 「导入这个会议音频，生成中文纪要，标注行动项和负责人」 |


## 二、系统工具 ⚙️
| 英文技能名 | 中文技能名 | 官方技能链接 | 核心功能（中文翻译） | 中文调用示例 |
|-----------|-----------|------------|----------------------|--------------|
| File Organizer | 文件自动整理 | [Clawdbot/file-organizer](https://clawdhub.com/skills/file-organizer) | 按类型/日期/大小分类文件，自动归档、重命名、删除过期文件 | 「整理下载文件夹，图片存到P盘，文档存到D盘，删除30天前的文件」 |
| Disk Cleaner | 磁盘清理工具 | [Clawdbot/disk-cleaner](https://clawdhub.com/skills/disk-cleaner) | 清理系统缓存、日志文件、临时文件，释放磁盘空间 | 「清理C盘缓存和日志文件，保留最近7天的重要日志」 |
| System Monitor | 系统监控助手 | [Clawdbot/system-monitor](https://clawdhub.com/skills/system-monitor) | 实时监控CPU/内存/磁盘使用率，异常时发送预警 | 「每小时检查一次CPU使用率，超过80%就推送到企业微信提醒我」 |
| Screenshot Tool | 截图自动化工具 | [Clawdbot/screenshot-tool](https://clawdhub.com/skills/screenshot-tool) | 全屏/区域截图、滚动截图，自动保存/分享/标注 | 「截取当前浏览器页面，标注重点区域，发送给产品部群」 |
| Batch Renamer | 批量重命名工具 | [Clawdbot/batch-renamer](https://clawdhub.com/skills/batch-renamer) | 按规则批量修改文件名（日期、序号、关键词替换） | 「把文件夹里的图片按“产品图-20240501-序号”重命名」 |


## 三、开发运维 🛠️
| 英文技能名 | 中文技能名 | 官方技能链接 | 核心功能（中文翻译） | 中文调用示例 |
|-----------|-----------|------------|----------------------|--------------|
| Code Generator | 代码生成器 | [Clawdbot/code-generator](https://clawdhub.com/skills/code-generator) | 按需求生成Python/Shell/Java代码，支持注释和基础调试 | 「生成一个Python脚本，读取Excel数据并导出为JSON格式」 |
| Log Analyzer | 日志分析工具 | [Clawdbot/log-analyzer](https://clawdhub.com/skills/log-analyzer) | 解析系统/应用日志，提取关键信息、排查错误、生成报告 | 「分析服务器日志，找出今天的错误信息并汇总成表格」 |
| API Tester | API 测试工具 | [Clawdbot/api-tester](https://clawdhub.com/skills/api-tester) | 发送HTTP请求（GET/POST）、验证响应结果、批量测试 | 「测试这个API：https://api.example.com/user，方法POST，参数name=test」 |
| Docker Manager | Docker 管理助手 | [Clawdbot/docker-manager](https://clawdhub.com/skills/docker-manager) | 启动/停止/重启Docker容器，查看容器状态、日志 | 「查看所有运行中的Docker容器，重启名称为moltbot的容器」 |
| Git Helper | Git 操作助手 | [Clawdbot/git-helper](https://clawdhub.com/skills/git-helper) | 执行Git命令（提交、推送、拉取、分支管理），简化操作 | 「提交当前项目的修改，备注“修复登录bug”，推送到main分支」 |


## 四、使用说明
1. **加载技能**：在 Moltbot 中发送指令 `加载技能：[中文技能名]`（如 `加载技能：邮件自动发送`），或通过命令行安装：
   ```bash
   # 从 Clawdbot 官方库安装技能
   moltbot skill install https://clawdhub.com/skills/[技能名]
调用技能：直接发送中文指令（如表格中的「中文调用示例」），Moltbot 会自动匹配对应技能执行。

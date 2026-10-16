# YouTube 科技大V · 播客/AI 视频监测

每天自动监测一批 YouTube 科技大V频道的播客对谈与 AI 相关视频，新增内容自动更新到此页面：

👉 **访问页面**：https://jiawen-w.github.io/youtube-ai-video-monitor/

## 监测频道

- **英文 AI 播客/博主**：Lex Fridman（Lex Fridman Podcast）、Dwarkesh Patel（Dwarkesh Podcast）、The AI Daily Brief、Machine Learning Street Talk、No Priors、Yannic Kilcher、AI Explained、Cognitive Revolution
- **官方/公司账号**：OpenAI、Anthropic、Google DeepMind、NVIDIA、Boston Dynamics、Figure、Unitree Robotics、Tesla（关注最新发布/演示/公告类视频）
- **中文科技大V**：李自然说、老石谈芯、阑夕、硅谷101

## 更新机制

- 豆包定时任务「YouTube大V播客监测」每天 10:30 触发
- 检索各频道最新播客对谈 / AI 视频 → 与历史推送去重 → 新增条目追加到 `videos.json` 并同步更新本仓库 → 自动 push，GitHub Pages 即时刷新
- 页面按发布日期倒序分组，支持按频道筛选

## 文件结构

| 文件 | 说明 |
|---|---|
| `index.html` | GitHub Pages 主页面（读取 `videos.json` 渲染） |
| `videos.json` | 结构化视频数据，每日追加 |

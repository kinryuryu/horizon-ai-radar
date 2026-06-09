# Horizon GitHub Actions + Pages 部署说明

这份说明适用于当前仓库这套 `DeepSeek + 中英双语 + AI 博主信息源` 配置。

## 当前已完成

- 已切换 AI 提供方为 `DeepSeek`
- 已配置 GitHub Actions 使用 `DEEPSEEK_API_KEY`
- 已开启定时任务
- 已设置为每天北京时间 `08:00` 自动运行一次
- 已保留 `workflow_dispatch`，可手动触发测试
- 已配置运行后发布到 `gh-pages` 分支

## 你需要做的事

### 1. 把仓库放到你自己的 GitHub 账号下

当前本地仓库的远程地址还是原作者仓库，不适合直接作为你的自动化发布仓库。

推荐做法：

1. 在 GitHub 新建你自己的仓库
2. 仓库名可以用 `horizon-ai-radar` 或你喜欢的名字
3. 把当前本地项目推送到你的仓库

### 2. 在 GitHub 仓库里配置 Secrets

打开：

`Settings > Secrets and variables > Actions`

至少新增这一个：

- `DEEPSEEK_API_KEY`

强烈建议再加这一个：

- `GITHUB_TOKEN_CUSTOM`

说明：

- `DEEPSEEK_API_KEY` 用于 AI 打分、摘要、背景补充
- 自带的 `GITHUB_TOKEN` 主要用于 Actions 写回仓库和部署 Pages
- 如果你希望 GitHub 信息源抓取更稳定，建议额外使用你自己的 GitHub Personal Access Token

## 推荐的 GitHub 抓取增强

如果要解决 GitHub Releases 抓取被限流的问题，建议额外做两步：

1. 创建一个 GitHub Personal Access Token
2. 把它保存为仓库 Secret：`GITHUB_TOKEN_CUSTOM`

然后把工作流里的环境变量 `GITHUB_TOKEN` 改成：

```yml
GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN_CUSTOM }}
```

如果不改，也能运行，只是 GitHub 相关新闻源可能会偶尔被限流。

## 3. 启用 GitHub Pages

打开：

`Settings > Pages`

设置：

- `Source`: `Deploy from a branch`
- `Branch`: `gh-pages`
- `Folder`: `/ (root)`

保存后，首次 Action 跑完就会生成站点。

## 4. 手动触发第一次运行

打开：

`Actions > Daily Horizon Summary`

点击：

- `Run workflow`

首次运行建议手动触发一次，确认：

- Action 成功
- `gh-pages` 分支已创建
- Pages 页面可以访问

## 成功后的结果

成功后你会得到：

- 一个每天自动更新的 GitHub Pages AI 新闻页
- `docs/_posts/` 下的日报 Markdown
- `data/summaries/` 下的原始摘要文件

## 可选下一步

后续还可以继续加：

- 飞书/Telegram 推送
- 更多 RSS 源
- Twitter/X 抓取
- 只保留中文输出
- 调整打分阈值，减少噪音

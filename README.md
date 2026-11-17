# 强化学习研究训练营

从智能体—环境接口、价值方法和策略梯度，逐步进入 RLHF、PPO、GRPO 与 Agentic RAG。

## 在线阅读

**[https://zhaojiew10.github.io/hands-on-rl-ebook/](https://zhaojiew10.github.io/hands-on-rl-ebook/)**

## 本书内容

### 第一部分 · 强化学习基础与价值方法

1. 强化学习基础：智能体—环境接口
2. 动态规划、蒙特卡洛与时序差分学习

### 第二部分 · 策略梯度与智能体实践

3. 面向电子游戏的 AI 智能体
4. REINFORCE、基线与广义优势估计

### 第三部分 · 大语言模型与智能体强化学习

5. 从零理解人类反馈强化学习（RLHF）
6. 使用 OpenRLHF 的 PPO 实战：Reddit 摘要器
7. 组相对策略优化（GRPO）
8. 基于强化学习的 Agentic RAG

## 本地阅读与构建

正文为 Markdown，本地预览不需要 GPU。

### Windows

在本目录执行：

```powershell
py -m venv .venv
.venv\Scripts\python -m pip install -r requirements.txt
.venv\Scripts\python -m mkdocs serve -a 127.0.0.1:8000
```

打开 <http://127.0.0.1:8000/>。按 `Ctrl+C` 停止服务。

### macOS / Linux

```bash
python3 -m venv .venv
.venv/bin/python -m pip install -r requirements.txt
.venv/bin/python -m mkdocs serve -a 127.0.0.1:8000
```

### 构建静态网站

```bash
python -m mkdocs build --strict
```

生成的网站位于 `site/`。`--strict` 会将文档警告视为错误，适合发布前检查。构建后可直接打开 `site/index.html`，或通过任意静态 HTTP 服务器托管 `site/`。

## 目录结构

```text
ebook/
├── docs/
│   ├── chapters/          # 8 个教程章节
│   ├── appendix/          # 课程资源导航与阅读说明
│   ├── resources/         # 静态资源
│   ├── stylesheets/       # 自定义样式
│   └── index.md           # 首页
├── mkdocs.yml             # MkDocs 配置与中文目录
├── requirements.txt       # 构建依赖
└── README.md
```

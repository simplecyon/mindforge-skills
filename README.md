# MindForge

一套结构化的思维技能包——不是给你更多答案，而是帮你在对的时刻用对的方式思考。

## 这是什么

MindForge 是一个**思维方法论技能包**，由 5 个互补的角色 + 1 个入口 skill 组成：

| Skill | 角色 | 核心动作 |
|---|---|---|
| `clarifier` | 澄清者 | 把模糊聊成清晰 |
| `muse` | 灵感触发器 | 给新角度和问题 |
| `thinker` | 深度分析 | 把一个角度想透 |
| `janus` | 批判审查 | 压力测试结论 |
| `conductor` | 指挥 | 收拢思维、做取舍 |
| `using-mindforge` | 入口 | 调度以上角色 |

## 思维节奏

```
模糊 → 清晰 → 发散 → 深入 → 质疑 → 收拢
 │       │       │       │       │       │
 │       │       │       │       │       └─→ /conductor
 │       │       │       │       └──────────→ /janus
 │       │       │       └──────────────────→ /thinker
 │       │       └──────────────────────────→ /muse
 │       └──────────────────────────────────→ (可以开工了)
 └──────────────────────────────────────────→ /clarifier
```

不是每段对话都需要走完全部流程。知道什么时候用什么，比什么都用更重要。

## 安装

### Claude Code

```bash
/plugin install mindforge
```

安装后，SessionStart hook 会在每次新会话开始时自动注入 `using-mindforge` 入口 skill——agent 不需要你手动触发就知道什么时候该用哪个角色。

### Codex CLI / OpenCode / Cursor / Gemini CLI

```bash
npx skills add simplecyon/mindforge-skills -g -y
```

### 手动安装

```bash
git clone https://github.com/simplecyon/mindforge-skills.git
# 将 skills/ 目录下的 skill 复制到你的 agent 的 skills 目录
```

## 快速开始

安装后，在对话中使用斜杠命令触发：

- `/clarifier` — 需求模糊时
- `/muse` — 需要新角度时
- `/thinker` — 要深入分析时
- `/janus` — 有了结论要质疑时
- `/conductor` — 想太多了要收拢时

## 设计理念

### 1. 思维有节奏，不是乱拳

每个 skill 有它的时刻。先澄清，再发散，再深入，再质疑，最后收拢。顺序可以跳，但不能乱。

### 2. 提问多于回答

最好的思考是被问出来的。这些 skill 不会给你答案，会给你更好的问题。

### 3. 移交要自然

每个 skill 结束时，如果判断该换角色了，会自然建议下一个。不打断节奏，不强推。

### 4. conductor 是收口

当思维进行了多轮，conductor 负责把散落的思维收拢成有用的东西——定位、蒸馏、取舍、方向。

## 与 Superpowers 的关系

MindForge 专注于**思维层面**——澄清、创意、分析、批判、决策。

[Superpowers](https://github.com/obra/superpowers) 专注于**执行层面**——计划、TDD、debug、code review。

两者互补，可以同时安装。

## License

MIT

# 副业体检仪 / Side Hustle Checker

> 判断一个赚钱机会，在现在这个时间点，对这个具体的执行者，究竟值不值得下场。
>
> Decide whether a money-making opportunity is worth pursuing for this particular person, at this particular moment.

[中文](#中文介绍) · [English](#english)

---

## 中文介绍

### 它是什么

副业体检仪是一个面向 Codex 和兼容 Agent Skills 工作流的决策 Skill，用于评估具体的副业、兼职、自由职业、小生意、个人产品、AI 赚钱项目或轻创业机会。

它不是副业推荐器，也不只判断“这个项目能不能赚钱”。它关注的是：

> **机会价值 = 项目质量 × 人项匹配 × 当前时机**

这是定性思考模型，不是机械评分公式。同一个项目，对不同的人，或者对同一个人的不同阶段，可能得到完全不同的结论。

### 它解决什么问题

- 这个副业值得我现在投入吗？
- 别人靠它赚钱，我是否也适合做？
- 这个兼职、接单机会或小生意值得接受吗？
- 一个 AI 赚钱项目究竟解决了真实问题，还是为了使用 AI 而制造需求？
- 两个副业之间应该选择哪个？
- 项目应该继续、做一次低成本实验，还是及时退出？
- 即使最后收入为零，我还能留下什么？

### 与普通“点子评分器”的区别

| 常见做法 | 副业体检仪 |
| --- | --- |
| 只分析项目是否有市场 | 同时分析项目、执行者和进入时机 |
| 根据少数成功案例判断机会 | 先检查证据强度、幸存者偏差和隐藏成本 |
| 输出虚假的精确分数或成功概率 | 使用可解释的定性结论 |
| 只看成功后的收益 | 同时运行失败收益测试 |
| 把所有机会包装成长期事业 | 允许诚实地标记为纯现金流项目 |
| 发现不会某项技能就直接否决 | 区分可学习缺口、前置门槛和不可接受缺口 |
| 不断扩展分析框架 | 使用 Analysis Breaker，在分析不再增值时进入行动 |
| 把 MVP 当成缩小版产品 | 只验证当前最大的单一未知 |

### 核心机制

#### 1. 证据检查

区分博主自述、收益截图等弱证据，与真实询盘、付款、订单和重复实验等强证据。一个成功案例只能证明“有人成功过”，不能证明普通执行者有较高成功概率。

#### 2. 项目 × 人 × 时机

项目本身不错，不代表适合你；适合你，也不代表现在就是最佳进入时机。Skill 会检查赚钱结构、真实成本、获客、交付、能力、资源、时间、可承受损失、偏好和当前阶段。

#### 3. 失败收益测试

假设项目最终收入为零：你还能带走作品、技能、代码、模板、客户认知、行业经验、数据或真实反馈吗？失败有所得，会提高低成本试错的价值；钱和时间都消失且没有沉淀，则应提高进入门槛。

#### 4. 第 100 次测试

如果把这件事做 100 次，第 100 次的你具体比第一次强在哪里？真正的复利可能来自行业理解、客户、数据、模板、组件、自动化和标准方案，而不只是更熟练地把需求转交给 AI。

#### 5. AI 必要性测试

从真实问题出发，按最简单有效的方式选择工具：

`简单规则 → Excel / 现成软件 → Python / 传统自动化 → API → LLM → Agent`

AI 只有在产生明显、可验证的效率或价值时才值得增加复杂度。

#### 6. Risk Breaker

优先检查知识产权、商标、肖像、学术诚信、隐私、数据安全、客户损失、平台规则、资金和法律监管风险。重大风险不可合理规避时，即使投入很低，也会给出风险否决；可以降险时，则优先寻找保留商业价值的相邻方案。

#### 7. Analysis Breaker

当风险可控、损失可承受、存在一定需求证据、失败仍有所得，且继续搜索不会明显提高决策质量时，停止增加 SWOT、PEST 或几十项评分，直接设计最低成本实验。

#### 8. 单一未知 MVP 与退出条件

一个首轮 MVP 只允许一个主要停止假设和一个可观察的通过/不通过门槛。投入上限、时间上限、成功信号、失败信号、复盘节点和停止条件都在行动前确定，避免沉没成本不断扩大。

### 可能给出的结论

| 结论 | 含义 |
| --- | --- |
| 🟢 值得下场 | 证据足够、风险可控、人与项目匹配，可以执行 |
| 🟢 值得 MVP | 方向有价值，但存在关键未知，需要低成本验证 |
| 🟡 值得观察 | 项目有价值，但当前证据、条件或时机不足 |
| 💰 纯现金流项目 | 可以赚钱，但能力或资产复利较弱 |
| 👤 好项目，但不适合你 | 项目不错，但与你当前条件、偏好或方向不匹配 |
| 🔴 建议放弃 | 综合成本明显高于潜在价值 |
| 🚨 风险否决 | 存在当前不值得承担的重大风险 |

### 安装

#### 方法一：克隆到 Codex Skills 目录

```bash
git clone https://github.com/lopezanthonyrdzwr5534-beep/side-hustle-checker.git ~/.codex/skills/side-hustle-checker
```

#### 方法二：手动安装

1. 下载仓库 ZIP。
2. 解压并将文件夹命名为 `side-hustle-checker`。
3. 将文件夹放入 `~/.codex/skills/`。
4. 确认入口文件位于 `~/.codex/skills/side-hustle-checker/SKILL.md`。
5. 重新打开任务或开始新一轮对话，让客户端重新发现 Skill。

### 使用

显式调用：

```text
$side-hustle-checker 我想做 AI 漫剧自营账号。我会剪辑，每周能投入 15 小时，最多愿意损失 200 元，值得做吗？
```

如果客户端支持隐式调用，也可以自然提问：

```text
这个副业适不适合我现在做？如果值得测试，请帮我设计一个有明确停止条件的最小实验。
```

信息不足且可能改变结论时，Skill 只会追问 1–3 个高价值问题，而不是发送一份冗长问卷。

### 输出结构

默认输出包括：结论、项目真正卖什么、为什么可能值得、真正成本、你与项目的匹配、失败后留下什么、第 100 次会变强在哪里、最大风险和下一步。

如果建议 MVP，还会给出一个只验证单一关键未知的最小实验，包括投入上限、时间上限、唯一成功门槛和停止条件。

### 项目结构

```text
side-hustle-checker/
├── README.md
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── diagnostic-framework.md
    └── behavioral-tests.md
```

- `SKILL.md`：触发边界、核心工作流和输出契约。
- `agents/openai.yaml`：Codex 界面元数据。
- `references/diagnostic-framework.md`：完整诊断框架。
- `references/behavioral-tests.md`：用于维护和回归验证的压力测试。

### 使用边界

本项目提供结构化决策支持，不保证项目盈利，也不能替代法律、财务、税务或其他专业意见。最终的价值排序和风险承受选择仍属于使用者。

---

## English

### What it is

Side Hustle Checker is a decision skill for Codex and compatible Agent Skills workflows. It evaluates a specific side hustle, freelance engagement, small business, personal product, AI money-making idea, or lightweight venture.

It is not a side-hustle recommendation engine, and it does not ask only whether an idea can make money. Its central model is:

> **Opportunity value = project quality × person–project fit × current timing**

This is a qualitative reasoning model, not a mechanical scoring formula. The same opportunity may deserve different conclusions for different people—or for the same person at a different stage.

### Questions it helps answer

- Is this side hustle worth my resources right now?
- Someone else is making money from it, but does it fit me?
- Should I accept this freelance job or small-business opportunity?
- Does this AI business solve a real problem, or is it looking for a problem merely because AI is available?
- Which of two side hustles should I choose?
- Should I continue, run a low-cost experiment, wait, or stop?
- If revenue ends up at zero, what will I still take away?

### How it differs from a typical idea scorer

| Typical approach | Side Hustle Checker |
| --- | --- |
| Evaluates whether a market exists | Evaluates the project, the person, and the timing together |
| Generalizes from a few success stories | Checks evidence strength, survivorship bias, and hidden costs first |
| Produces a precise-looking score or success probability | Uses explainable qualitative verdicts |
| Counts only upside | Runs a failure-return test as well |
| Treats every opportunity as a potential long-term company | Allows an honest “cash-flow project” classification |
| Rejects the user for lacking a skill | Separates learnable gaps, prerequisites, and unacceptable gaps |
| Keeps adding analysis frameworks | Uses an Analysis Breaker when more analysis no longer improves the decision |
| Treats an MVP as a smaller complete product | Tests the single biggest current unknown |

### Core mechanisms

#### 1. Evidence check

The skill separates weak evidence—creator claims, revenue screenshots, and isolated success stories—from stronger evidence such as real inquiries, payments, orders, operating data, and repeated experiments. Proof that someone succeeded is not proof that an ordinary entrant has a high probability of success.

#### 2. Project × person × timing

A good project may not fit you, and a project that fits you may still have the wrong timing. The skill examines economics, hidden costs, acquisition, delivery, skills, resources, sustainable time, acceptable loss, work preferences, and current life stage.

#### 3. Failure-return test

Assume final revenue is zero. Do you still keep a portfolio piece, a skill, code, templates, customer insight, industry knowledge, data, or real feedback? A dense failure return makes a low-cost experiment more valuable. Losing money and time with nothing reusable raises the entry threshold.

#### 4. The 100th-repetition test

If you perform the work 100 times, how is the person doing repetition 100 concretely stronger than the person doing repetition one? Compounding may come from domain knowledge, customers, data, templates, components, automation, and standardized solutions—not merely from becoming faster at passing requests to AI.

#### 5. AI necessity test

Start with the real problem and choose the simplest tool that solves it:

`simple rules → Excel / existing software → Python / traditional automation → API → LLM → agent`

AI should add complexity only when it creates clear, testable value or efficiency.

#### 6. Risk Breaker

The skill checks intellectual property, trademarks, likeness rights, academic integrity, privacy, data security, customer harm, platform rules, financial exposure, and legal or regulatory risk. If a major risk cannot be reduced reasonably, the opportunity receives a risk veto even when the monetary experiment is small. When possible, it proposes a safer adjacent offer that preserves the core value.

#### 7. Analysis Breaker

When risk is controlled, loss is affordable, some demand evidence exists, failure still leaves useful assets, and further research will not materially improve the decision, the skill stops adding SWOTs and elaborate scoring systems and moves to a real experiment.

#### 8. Single-unknown MVP and exit trigger

The first MVP must have exactly one primary stopping hypothesis and one observable pass/fail gate. Spending, time, success signal, failure signal, review point, and stopping condition are written before action begins, reducing the pull of sunk costs.

### Possible verdicts

| Verdict | Meaning |
| --- | --- |
| 🟢 Worth entering | Evidence is sufficient, risk is controlled, and the person–project fit is strong |
| 🟢 Worth an MVP | The direction has value, but one critical unknown needs a low-cost test |
| 🟡 Worth watching | The opportunity has value, but evidence, conditions, or timing are insufficient |
| 💰 Cash-flow project | It may make money, but capability or asset compounding is limited |
| 👤 Good project, wrong person | The business may be sound, but it conflicts with the user's current conditions, preferences, or direction |
| 🔴 Recommend dropping | Total cost is clearly greater than the likely value |
| 🚨 Risk veto | A material risk is not worth accepting in the current form |

### Installation

#### Option 1: Clone into the Codex Skills directory

```bash
git clone https://github.com/lopezanthonyrdzwr5534-beep/side-hustle-checker.git ~/.codex/skills/side-hustle-checker
```

#### Option 2: Install manually

1. Download the repository as a ZIP file.
2. Extract it and name the folder `side-hustle-checker`.
3. Place the folder under `~/.codex/skills/`.
4. Confirm that the entry point is `~/.codex/skills/side-hustle-checker/SKILL.md`.
5. Open a new task or start another conversation turn so the client can discover the skill.

### Usage

Explicit invocation:

```text
$side-hustle-checker I want to run my own AI comic-drama account. I can edit video, have 15 hours per week, and can afford to lose $30. Is it worth testing?
```

Clients that support implicit invocation may also accept a natural request:

```text
Does this side hustle fit me right now? If it deserves a test, design the smallest experiment with a firm stopping condition.
```

When missing information could materially change the verdict, the skill asks only one to three high-value questions instead of presenting a long questionnaire.

### Output

The default response covers the verdict, what the opportunity really sells, why it may be worthwhile, hidden costs, person–project fit, failure returns, the 100th-repetition outcome, the largest risks, and one next action.

When the verdict is “Worth an MVP,” the response adds a minimum experiment that tests one critical unknown, with a spending cap, time limit, single success gate, and stopping condition.

### Repository structure

```text
side-hustle-checker/
├── README.md
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── diagnostic-framework.md
    └── behavioral-tests.md
```

- `SKILL.md`: activation boundaries, core workflow, and output contract.
- `agents/openai.yaml`: Codex-facing metadata.
- `references/diagnostic-framework.md`: the complete diagnostic framework.
- `references/behavioral-tests.md`: maintenance and regression scenarios.

### Scope and disclaimer

This project provides structured decision support. It does not guarantee profit and does not replace legal, financial, tax, or other professional advice. The user's value priorities and risk tolerance remain their own decisions.

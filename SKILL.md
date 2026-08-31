---
name: geo-strategy-init
description: Initialize and formulate GEO (Generative Engine Optimization) strategy for brands. Use when the user needs to create a GEO strategy, plan GEO optimization directions, conduct brand research for GEO purposes, or formulate AI-search brand presence strategy. Triggers on keywords like "GEO策略", "GEO研判", "GEO规划", "AI搜索优化", "品牌GEO", "GEO方向", or when the user uploads brand materials requesting GEO strategy formulation. Also covers GEO platform selection (平台打法/平台优先级/平台矩阵) via the six-platform AI ecosystem source-preference reference, GEO 的商务定位, and the Query Set 定词方法论 (references/query-set-methodology.md: 品牌可触发 BTR 预检、五类决策意图、两阶段分层、四层转译、伪命题识别、语义簇去重、指标与测量纪律)（GEO 怎么卖、要不要单独推 GEO、GEO 作为需求入口撬动传播案——见 v4.4）。This skill guides a structured workflow from brand research to GEO strategy output.
---

# GEO研判策略初始化

Structured workflow for formulating brand GEO strategies. Covers strategy positioning questionnaire → AI answer scanning → brand deep-dive research → GEO opportunity diagnosis → search chain mapping → strategy direction generation → deliverable output.

> **Core logic upgrade (v4.0)**: GEO is not "produce content and wait for AI to cite". It is "scan how AI currently answers → identify brand absence nodes → produce targeted content to correct/occupy". The further upgrade: GEO is not keyword optimization — it is consumer intent re-expressed in the AI world. The further upgrade: GEO strategy must be **future-oriented**, anchored to the brand's **recent strategic signals** (official communications, executive statements, annual reports), not a summary of past product practices. Read `references/boundary-rules.md` before execution. Read `references/geo-methodology.md` Section 4 for the six intent derivation methodologies.

> **v4.1 补充**：示例词是对客信任的第一载体。所有词表必须过 Step 3C「示例词质量红线」（品牌可答性、短词优先、真实口吻、渠道自营/白牌对比词），尤其是轻量方向/初步沟通方案。

> **v4.2 补充**：业务模式决定方向完整性。品牌含加盟/特许经营/经销招商模型时，方向清单必须含一个 B 端招商方向（潜在加盟商是独立于消费者的搜索人群），并与 C 端信息纠偏方向联动——规则与词层模式见 Step 3B「业务模式必查」。

> **v4.3 补充**：平台选择有据可依。链路各层「Adapted platform」与交付物的平台打法章节，一律依据 `references/platform-preferences.md`（六大平台信源/内容形态偏好 + 按方向受众选平台启发式，2026-08 快照）——不做全平台覆盖，选 2–3 个核心平台深耕，其余跟随覆盖。

> **v4.4 补充（GEO 的商务定位）**：GEO 单独作为一个需求去推进很难成立，它的正确定位是**需求入口**——敲门砖、信任凭证、谈判桌上的专业座位，而不是主菜（用户 2026-08-04 提出的倾向，2026-08-14 一鸣武汉案完整验证：GEO 方案敲开门，成交的是 50 万传播案，GEO 嵌为三板块之一）。三条落地推论：
> 1. **悖论：GEO 的价值在「不主推它」的那一刻兑现。** 用 GEO 的专业性证明懂，再用主动不推 GEO（如建议阶段一不做指定词、先做传播）证明不贪心——两者相加才换来更大的盘子。抱着词包不放，会就开成普通供应商见面会。
> 2. **别把结论推过头。** 入口型产品的专业门槛不能降——越不做主菜，越要显得深。现场接不住第二层追问（结构性文章怎么写、信源偏好、平台差异、合规边界），入口立刻变减分项。
> 3. **交付里的落位是「收口/放大器」而非主角。** 传播案里 GEO 的角色：事件造声量、矩阵立权威、GEO 收成果——所有声量最终在 AI 搜索端沉淀成可见结果。方案结构与报价比重按此逻辑排（GEO 占小头但角色讲透），不要把 GEO 写成独立主推需求。

> **v4.5 补充（定词层标准化）**：引入 `references/query-set-methodology.md` 作为 Query Set 生产规范（巴拉巴拉案实战沉淀）。方向是骨架、定词是肌肉——词表必须过「真实消费问题 × 品牌可触发 × 品牌可证实」最小闭环。对既有流程的三处硬升级：
> 1. **示例词/链路词先做 BTR 预检再进表**：只出知识不出品牌的问法删除或改写（Step 3C 第 1 条升级为可测的 Brand Trigger Rate，不再只凭自检印象）。
> 2. **词表按语义簇（Cluster ID）去重管理**：同义问法是簇内变体不是多个战场；覆盖度按簇计算，不按句子数虚增。
> 3. **意图与阶段结构化**：候选词按五类决策意图（推荐/比较/购买决策/场景/品牌验证）× 两阶段（从知道到入选/从入选到偏爱）归位；Phase 2 方向少而精，不围绕品牌理念造词。指标层同步升级为「输入质量 + 认知校准 + 推荐抢位」三层，替代原「链路覆盖度/可见性/信任度/好感度」笼统四维。

## Workflow Overview

Execute in five phases. Do not skip phases unless user explicitly requests otherwise.

```
Pre-Phase: Strategy Positioning Questionnaire (MANDATORY)
Phase 0: AI Answer Status Scan (with intent-layer analysis)
Phase 1: Brand Deep-Dive Research (with parallel-world migration + strategic forward-looking)
Phase 2: GEO Opportunity Diagnosis
Phase 3: Search Chain Mapping & Strategy Formulation (with pre-validation + future-orientation)
Phase 4: Strategy Document Output
```

---

## Pre-Phase: Strategy Positioning Questionnaire (MANDATORY)

> **Purpose**: Different brands and different internal teams have fundamentally different GEO objectives. A crisis-ridden brand needs reputation defense; a new brand needs category education; a mature brand needs competitive interception. This questionnaire ensures subsequent strategy work is anchored to the right objective — not a one-size-fits-all template.

Before executing any research or scanning, present the following 4 questions to the user. Use the `ask_user` tool with single/multi-select format. Do not proceed until user has responded.

### Question 1: Brand Type & Stage (single-select)

**Question**: 当前品牌处于什么阶段？

| Option | Stage | Typical GEO Objective |
|--------|-------|----------------------|
| A | **新锐品牌**（0-3年，市场认知度低） | 建立基础认知：让AI能准确回答"XX是谁" |
| B | **成长期品牌**（3-7年，快速扩张中） | 心智占位：在品类问询中被优先提及 |
| C | **成熟品牌**（7年+，市场地位稳固） | 防御+优化：巩固地位、修复过时信息 |
| D | **危机/转型期品牌**（面临负面或战略调整） | 声誉管理：控制AI如何解释品牌 |
| E | **出海品牌**（主攻海外市场） | 跨市场认知：在新市场建立品牌定义 |

### Question 2: Internal Team Function (single-select)

**Question**: 推动GEO的内部团队是什么职能？

| Option | Team | Typical GEO Focus |
|--------|------|------------------|
| A | **品牌部/Marketing** | 品牌故事传达、心智占位、情感连接 |
| B | **公关部** | 声誉管理、负面防御、危机应对 |
| C | **电商/增长团队** | 转化链路、购买决策拦截、ROI导向 |
| D | **产品团队** | 产品差异化传达、功能卖点占位 |
| E | **高管/战略层** | 全局品牌资产建设、竞争格局 |
| F | **外部代理商**（代品牌方做GEO） | 综合：需兼顾上述多方诉求 |

### Question 3: Primary GEO Objective (multi-select, max 2)

**Question**: 本次GEO策略最希望解决什么问题？（最多选2项）

| Option | Objective | Strategy Implication |
|--------|-----------|---------------------|
| A | **防御型**：防止AI输出错误/过时/负面品牌信息 | 优先做信息审计+事实库建设 |
| B | **进攻型**：在竞品对比中被AI优先推荐 | 优先做竞品截流+差异化占位 |
| C | **教育型**：建立新品类/新概念的AI认知 | 优先做品类教育+概念定义 |
| D | **修复型**：纠正AI中已有的错误品牌描述 | 优先做内容覆盖+信源治理 |
| E | **占位型**：提升品牌在AI回答中的整体可见度 | 优先做链路全覆盖+内容矩阵 |
| F | **出海型**：在海外市场建立品牌AI认知 | 优先做跨语言信源+本地化内容 |

### Question 4: Strategy Depth & Deliverable (single-select)

**Question**: 期望的策略深度和交付物形式？

| Option | Depth | Deliverable |
|--------|-------|-------------|
| A | **轻量方向**（快速定方向+示例词） | 策略方向清单 + 三层意图示例词 |
| B | **标准研判**（完整GEO策略） | 品牌调研摘要 + 诊断 + 链路地图 + 策略方向 |
| C | **深度方案**（可执行的全案） | 完整研判 + 内容矩阵 + 执行计划 + 监测方案 |
| D | **可视化交付**（用于客户汇报） | 标准/深度内容 + PPT格式输出 |

---

### Questionnaire Result Application

After receiving user responses, apply the following **Strategy Orientation Matrix** to calibrate all subsequent phases:

**Brand Stage × Team Function → Strategy Priority Override**:

|  | 品牌部 | 公关部 | 电商/增长 | 产品团队 | 高管/战略 | 代理商 |
|--|--------|--------|-----------|----------|-----------|--------|
| **新锐品牌** | 品牌故事+品类教育 | 基础信任建设 | 转化链路搭建 | 产品定义 | 品牌资产规划 | 全案统筹 |
| **成长期** | 心智抢占+差异化 | 声誉监测+预防 | 竞品截流 | 功能卖点 | 格局卡位 | 增长导向 |
| **成熟期** | 品牌刷新+年轻化 | 危机防御+修复 | 场景扩展 | 新品类教育 | 护城河巩固 | 综合攻防 |
| **危机/转型** | 叙事重建 | 负面管控+对冲 | 信心修复 | 信息澄清 | 战略重塑 | 全维度修复 |
| **出海** | 跨文化品牌定义 | 海外舆情管理 | 本地化转化 | 产品适配 | 市场进入策略 | 全球化统筹 |

**Primary Objective → Phase Adjustment**:

| 主要目标 | Phase 0 调整 | Phase 1 调整 | Phase 2 重点 | Phase 3 重心 |
|---------|-------------|-------------|-------------|-------------|
| 防御型 | 重点扫负面/错误信息 | 深挖危机历史 | 声誉风险评估 | 防御性内容矩阵 |
| 进攻型 | 重点扫竞品对比场景 | 深挖竞品策略 | 竞品差距分析 | 截流型链路地图 |
| 教育型 | 重点扫品类认知空白 | 深挖品类定义 | 认知缺口诊断 | 教育型内容体系 |
| 修复型 | 重点扫错误描述 | 深挖信息源头 | 错误归因分析 | 覆盖型内容铺设 |
| 占位型 | 全链路扫描 | 全面调研 | 全局缺位诊断 | 全覆盖链路地图 |
| 出海型 | 重点扫海外AI平台 | 深挖海外市场 | 跨市场差距分析 | 本地化链路地图 |

**Deliverable Depth → Output Scope**:

| 深度 | Phase 执行范围 | 输出内容 |
|------|---------------|---------|
| 轻量方向 | Phase 1 精简 + Phase 3 直接出方向 | 3-5个策略方向 + 三层意图示例词（每方向3短词+2长词，必须过 Step 3C 示例词质量红线） |
| 标准研判 | 全Phase执行 | 调研摘要 + 诊断 + 链路地图 + 策略方向 |
| 深度方案 | 全Phase + 增强版Phase 3 | 上述全部 + 内容矩阵 + 执行计划 + 监测方案 |
| 可视化交付 | 全Phase + 格式转换 | 上述全部 + PPT格式 |

Document the questionnaire results at the top of the final deliverable under a「策略定位」section.

---

## Phase 0: AI Answer Status Scan

**Input**: Brand name, core category, target audience
**Output**: Summary of how AI currently answers key questions, citation sources, brand absence nodes

Before any research or strategy work, first simulate or search how mainstream AI platforms (DeepSeek, Doubao, Wenxin Yiyan, Tongyi, Kimi) answer questions related to this brand and its category.

> **Methodology anchor**: Apply `Intent Layer Derivation` (geo-methodology.md §4.1 Method 2) and `Question Diversity Exhaustion` (geo-methodology.md §4.1 Method 3). Do not scan only brand-layer questions — you must cover all three intent layers.

> **Pre-Phase calibration**: Adjust scan focus based on questionnaire results (see Strategy Orientation Matrix above). If user selected "防御型", prioritize scanning for negative/misleading answers. If "进攻型", prioritize competitive comparison scenarios.

**Three-layer intent scanning model**:

| 意图层级 | 消费者心理状态 | 扫描时应覆盖的问题类型 |
|---------|--------------|---------------------|
| **第一层（疑虑层）** | "我要不要做这个事？" | "XX还值得买吗？""现在还有必要XX吗？" |
| **第二层（品类层）** | "有什么选择？" | "有哪些品牌适合XX？""XX牌子推荐" |
| **第三层（品牌层）** | "AB之间选哪个？" | "XX和YY怎么选？""XX靠谱吗？" |

For each key question, document:

| 扫描维度 | 记录内容 |
|---------|---------|
| **用户问题** | 消费者实际会问的典型问题（覆盖三层意图的3-5层递进） |
| **AI当前回答** | AI怎么回答这个问题？提到了哪些品牌？怎么描述本品牌？ |
| **引用来源** | AI引用了哪些信源？（百科/知乎/小红书/新闻/电商等） |
| **品牌缺位节点** | 本品牌在哪些关键问题上未被提及 / 被错误描述 / 被竞品压制？ |

**Question diversity requirement**: For each core intent, exhaust at least 5 question variants (audience dimension, scenario dimension, emotional dimension, decision-stage dimension, functional dimension). See geo-methodology.md §4.1 Method 3 for the variant matrix.

**Purpose**: This scan serves as the **reverse basis** for content production. All subsequent strategy work is grounded in these real gaps, not theoretical assumptions.

Read `references/geo-methodology.md` Section 6 for detailed scanning methodology.

---

## Phase 1: Brand Deep-Dive Research

Read `references/brand-research-framework.md` first. Execute all modules:

1. **Core Brand Identity** (Module 1) — 200-word summary
2. **Brand DNA & Founding Philosophy** (Module 2) — origin story, founder imprint
3. **Brand Evolution** (Module 3) — 3-5 phases, last 2 years in detail
4. **Product Line Strategy Matrix** (Module 4) — 3-4 core product lines
5. **Brand Communication System** (Module 5) — visual identity, tone, content strategy
6. **Competitive Landscape** (Module 6) — mindshare, sentiment, crisis history
7. **Brand Moat & Outlook** (Module 7) — defensible assets, growth opportunities
8. **GEO-Specific Supplement** (Module 8) — business model, financial report review, PR actions, challenges
9. **Strategic Forward-Looking Analysis** (Module 9, v4.0 MANDATORY) — recent strategic signals, future direction

> **v4.0 核心升级 - Module 9 是策略方向的唯一锚点**：
> - 必须从品牌**近一年/半年**的对外发声（官方矩阵号、高管发言、权威渠道）中提炼战略信号
> - 上市企业必须研读财报「管理层讨论与分析」板块的战略方向声明
> - **禁止**基于历史产品矩阵（如"全场景产品矩阵"）推导GEO方向
> - 所有策略方向必须回答"品牌未来想成为什么"，而非"品牌过去做了什么"
> - Module 9 的输出应包含：品牌自我定义、品牌要去哪里、品牌在解决什么问题、品牌的差异化赌注

**Research requirements beyond the framework:**
- 充分研究品牌近一年的公关方向和动作
- 梳理品牌现实困境与挑战
- 上市公司必须研读财报「管理层讨论与分析」
- 明确品牌的具体业务模式与类型（DTC/经销/加盟/平台/B2B等）；含加盟/招商模型的，Phase 3 必须产出 B 端招商方向（见 Step 3B「业务模式必查」）
- 所有 brand actions must be cross-verified with同期业务进展
- **v4.0 新增**: 系统翻阅品牌官方矩阵号近6个月内容，提炼战略关键词

> **Methodology anchor**: Apply `Parallel World Migration` (geo-methodology.md §4.1 Method 1). During research, actively translate physical-world consumer insights into AI-world question patterns. Document: "Based on [user insight], consumers would likely ask AI..."

> **Pre-Phase calibration**: If questionnaire indicates "轻量方向" deliverable,精简 Phase 1 to 核心品牌摘要 + 战略前瞻(Module 9) + 竞品格局 only. Skip detailed brand evolution and communication system analysis.

**Output**: A structured《品牌深度调研报告》with GEO-specific insights and **Strategic Forward-Looking Summary (Module 9)** appended. The Module 9 summary must be prominently featured as the strategic anchor for all subsequent phases.

---

## Phase 2: GEO Opportunity Diagnosis

Read `references/geo-methodology.md` for the dual-dimension framework (Market × PR).

Based on the research report + Phase 0 scan results, diagnose:

| 诊断维度 | 关键问题 |
|---------|---------|
| **可见性** | 品牌在主流AI平台的当前能见度如何？ |
| **信息准确性** | AI回答中的品牌信息是否准确？是否存在错误/过时/矛盾信息？ |
| **竞品对比** | 竞品是否已做GEO？其在AI搜索中的表现 vs 本品牌？ |
| **声誉风险** | 是否存在历史负面信息可能被AI聚合呈现？ |
| **内容体系** | 品牌内容是否结构化、一致、可信？跨部门/跨平台是否存在矛盾？ |
| **场景覆盖** | 品牌核心场景/人群需求在AI搜索中是否被覆盖？ |
| **链路缺位** | 从泛需求到精准决策的搜索链路中，品牌在哪些节点缺失？ |
| **战略缺位** (v4.0 新增) | 品牌未来战略方向在AI搜索中是否被覆盖？AI是否知道品牌"要去哪里"？ |

> **Methodology anchor**: Apply `Source Anchoring` (geo-methodology.md §4.1 Method 4). For each diagnosis finding, map back to physical-world sources. Ask: "Which real-world source is causing this AI-world problem?"

> **Pre-Phase calibration**: Prioritize diagnosis dimensions based on user's Primary GEO Objective. If "防御型", elevate 声誉风险 and 信息准确性 to top priority. If "进攻型", elevate 竞品对比 and 链路缺位.

> **v4.0 新增诊断维度 - 战略缺位**: 检查品牌近期对外传递的战略方向（如"科技护肤""下沉市场""东方美学"）在AI搜索中是否被反映。如果AI回答中完全没有这些战略信号，这是最高优先级的缺位。

**Output**: A《GEO诊断摘要》listing top 3-5 priority problems to solve, with **strategic absence flagged as highest priority if present**.

---

## Phase 3: Search Chain Mapping & Strategy Formulation

**This phase replaces the old "keyword list" approach with a "search chain map" approach.**

> **v4.0 核心红线 - 前瞻性约束**：
> - 策略方向必须锚定 Module 9 提炼的品牌未来战略，**禁止**基于历史产品矩阵总结方向
> - 方向命名格式："[未来战略方向] → [GEO心智目标]"，**禁止**"[已有产品线] → [产品覆盖]"
> - 典型错误方向（需删除重写）："全场景产品矩阵""全线产品占位""产品品类全覆盖"
> - 正确方向示例：「专利技术壁垒 → 建立科技护肤专家心智」「东方美学差异化 → 建立文化品牌心智」

> **Methodology anchor**: Apply `Pre-Validation > Post-Optimization` (geo-methodology.md §4.1 Method 5). Before building any chain map, validate that the identified intents are real consumer questions — not brand assumptions. Reference the vodka case study in geo-methodology.md.

> **Pre-Phase calibration**: Strategy direction count and depth vary by deliverable level:
> - 轻量方向: 3-5个方向, 每方向3短词+2长词（对客初步沟通规格，逐条过 Step 3C 质量红线）
> - 标准研判: 4-5个方向, 完整链路地图
> - 深度方案: 5个方向 + 内容矩阵 + 执行计划

Read `references/strategy-examples.md` for format reference. Read `references/geo-methodology.md` Section 6 for chain mapping methodology.

### Step 3A: Build Search Chain Maps

> **v4.5 定词规范**：链路各层的「Typical user question」按 `references/query-set-methodology.md` 生产——四层转译（品牌资产→消费者问题→Query→RTB）逐层可追溯，候选词过 BTR 预检与一票否决清单（§1/§5），同义词按语义簇去重（§6），场景词必须带「人群+场景+矛盾+品牌槽位」结构（§7）。深度方案的完整词表按 §8 工作表字段输出。

For each strategy direction, construct a **progressive search chain** covering 3-5 layers from broad demand to precise decision:

```
第一层（泛需求/疑虑层）：用户问什么 → AI怎么答 → 品牌是否被提及 → 占位策略
第二层（品类认知层）：...
第三层（对比/疑虑层）：...
第四层（精准决策层）：...
第五层（售后/验证层）：...
```

Each layer must include:
- **Typical user question** (conversational prompt style, reflecting real consumer language)
- **Intent classification** (which of the 3 intent layers this question belongs to)
- **AI current answer summary** (from Phase 0 scan)
- **Brand presence status** (present / absent / misrepresented)
- **Occupation priority** (P0 must-occupy / P1 recommended / P2 optional)
- **Content angle suggestion**
- **Adapted platform** — 平台选择依据 `references/platform-preferences.md`（v4.3）：按该层受众与意图匹配平台信源偏好，不凭印象分配

### Step 3B: Generate Strategy Directions

Generate 3-5 GEO strategy directions. Each direction must follow:

> **[品牌未来战略方向]** → **[GEO心智目标]**

> **v4.0 命名规则升级**：
> - 前半部分必须是品牌**未来战略方向**（从Module 9提炼），而非已有产品/资产
> - 后半部分是GEO要达成的**心智目标**
> - 整体构成一个"品牌未来要成为X，所以GEO要在AI中建立X认知"的逻辑链
> - ❌ 错误：「全场景产品矩阵 → 覆盖全品类搜索」
> - ✅ 正确：「真奶真茶原料标准 → 建立品质新茶饮心智」

For each direction, output:
1. **核心逻辑** — why this direction, grounded in **Module 9 strategic signals** (not product summaries)
2. **战略信号支撑** — which specific recent brand communication/executive statement/annual report finding supports this direction (v4.0 MANDATORY)
3. **搜索链路地图** — 3-5 layer progressive chain (from Step 3A)
4. **节点占位评级** — each chain node rated P0/P1/P2
5. **内容角度建议** — what "standard answer" to prepare at each node
6. **核心信息锚点** — brand facts AI answers must include

**Key constraints:**
- Directions must be customized per brand — do not mechanically copy from examples
- Chain nodes must reflect actual user search progression (broad → comparative → decision → validation)
- **Each chain must cover all three intent layers** (疑虑层 → 品类层 → 品牌层), per geo-methodology.md §4.1 Method 2
- Each node prepares a "standard answer" for AI to cite, not just a keyword
- Prioritize directions that address the highest-impact problems from Phase 2 diagnosis
- Apply the **Six-Methodology Checklist** (geo-methodology.md §4.2) before finalizing directions
- **v4.2 业务模式必查（MANDATORY，2026-08-04 对客初步沟通稿纠正沉淀）**：Phase 1 Module 8.1 判定品牌含**加盟/特许经营/经销招商**模型时，方向清单必须包含一个 **B 端招商方向**（如「加盟招商与经营信任 → 建立"可信赖加盟标的"心智」）。漏掉它的典型后果：初稿全是 C 端方向，被客户要求补加。执行要点：
  - 潜在加盟商是独立于消费者的搜索人群，词层自有意图结构——决策层：「XX加盟费多少」「加盟XX赚钱吗」「XX加盟靠谱吗」「回本周期多久」「XX和竞品加盟哪个好」；品类层：「开XX店加盟哪个牌子好」；疑虑层：「XX不是在关店吗，现在加盟会不会砸手里」
  - 战略信号锚点用拓店规划、单店模型优化、供应链扶持、新市场开放加盟等 Module 9 素材，不用历史门店数堆砌
  - **与 C 端信息纠偏方向联动**：C 端负面叙事（关店潮、食安、股价波动）不纠偏，B 端信任建不起来——优先级排序时两个方向绑定评估
- **v4.0 前瞻性红线 (MANDATORY)**:
  - [ ] 每个方向是否锚定于 Module 9 的未来战略？
  - [ ] 方向命名是否使用"[未来战略方向] → [GEO心智目标]"格式？
  - [ ] 是否有任何方向基于"全场景产品矩阵"等总结性表述？（如有，删除重写）
  - [ ] 每个方向是否能在品牌近半年官方发声中找到战略信号支撑？
  - [ ] 方向是否回答"品牌未来想成为什么"而非"品牌过去做了什么"？
  - [ ] 品牌含加盟/招商模型时，是否已有 B 端招商方向并与 C 端纠偏方向联动？（v4.2）

### Step 3C: 示例词质量红线（v4.1，2026-07 对客初步方案多轮纠正沉淀）

> **v4.5 升级**：本步骤红线与 `references/query-set-methodology.md` 合并执行——第 1 条「品牌可答性」升级为 **BTR 预检**（多平台实测，记录平台/模型/日期；样本不足标「小样本预检」）；第 2/3 条口吻要求用方法论的「消费者真实性」清单复核；词表结构按五类意图 × 两阶段归位，覆盖度按语义簇计算。伪命题（纯科普词/品牌方价值词/ESG 直译词）按方法论 §5 一票否决。

示例词是客户判断 GEO 专业度的第一眼证据——方向骨架再对，词没人味就是哑弹。以下每条都被真实对客沟通纠正过，生成词表时逐条必过：

1. **品牌可答性校验（最高优先级）**：每个示例词必须是"AI 回答时有位置放品牌名"的问题。纯科普/功能类词（如「保鲜膜什么材质最安全」）AI 只输出功能知识、不带任何品牌——这是词表通病。要么改造成决策型问法（「…什么牌子好」「…哪个品牌靠谱」），要么删除。自检：把词丢给通用 AI，看回答里能否自然出现品牌。
2. **初步沟通方案＝短词优先**：初次给客户的词表以短词为主（显聚焦、显真实量级），**每方向 3 短词 + 2 长词**即可。长词过多会被客户挑战"这种问法的人很少""词是为了凑逻辑造出来的"。长尾问法留到深度方案阶段再铺。
3. **真实感 > 方法论正确**：示例词必须像真实消费者原话（口语、带场景、带人群自称），让客户一眼认出"这就是我家用户会问的"。营销人腔（「适合精致露营场景的一次性餐具解决方案」）一律重写；品牌官方英文名/别名不露出（没有人问 AI 时会说「佳能（Glad）」）。
4. **对比词覆盖渠道自营与白牌**：竞对词不只列传统品牌，必须纳入山姆/盒马等渠道自营和白牌——它们在用渠道信任截流，是成熟品牌真实的价格心智威胁。
5. **独家心智位占位**：方向设计主动挖掘竞品无法复制的独家心智资产（两代人共认的代际信任、事件后自查自纠的事实链、环保材质等 ESG 资产），示例词围绕抢占这些位置设计。
6. **产品事实词先核对再写**：涉及产品事实的示例词（能否微波、材质、适用人群/宠物禁忌）必须与官方产品资料核对，不凭常识推断。
7. **不承诺"真实搜索量"**：词表说明禁止写「短词是流量盘，代表真实搜索量」这类断言——AI 平台没有公开搜索量数据，写上会被客户质疑且解释成本大。词表只标注意图层级与策略目的。

> **轻量方向定位（弹药不是货）**：初步沟通阶段的 GEO 内容是证明专业度的弹药，不是交付物本身。深度不必重，但示例词必须惊艳真实——客户对 GEO 的信任全部由词表质感建立。

---

## Phase 4: Strategy Document Output

Compile the final《品牌GEO研判策略》document in this structure:

```
一、策略定位（Pre-Phase 问卷结果摘要）
二、AI回答现状扫描（Phase 0 核心发现）
三、品牌深度调研摘要（Phase 1 核心结论）
    3.1 品牌基本面摘要
    3.2 战略前瞻分析（Module 9 核心发现 - v4.0 新增）
四、GEO现状诊断（Phase 2 核心结论）
五、GEO搜索链路地图与策略方向（Phase 3 完整输出）
    5.1 链路总览
    5.2 策略方向一：[未来战略方向] → [GEO心智目标]
        - 核心逻辑
        - 战略信号支撑（v4.0 新增）
        - 搜索链路地图 + 节点占位 + 锚点
    5.3 策略方向二：...
    5.4 策略方向三：...
六、衡量指标建议（v4.5 起按 query-set-methodology.md §9 三层指标体系：输入层 Query 质量 / 认知校准层 / 推荐抢位层，并按两阶段映射主辅指标；遵守 §9.5 测量纪律）
七、风险防御与合规建议
八、执行优先级与时间建议
九、边界声明与交付物说明
```

**Output format**: Markdown by default. Adapt to user's requested format (PPT/Word/等) if specified.

**Style**: INTJ — professional, concise, cut to the chase. No filler. Every sentence must carry strategic value.

**Boundary statement** (must include in deliverable):
- 本策略承诺「搜索链路覆盖度」和「内容占位策略」，不承诺AI引用效果
- 平台优先级作为可配置参数，需人工定期更新
- 关键决策节点（优先级排序、竞品截流、预算分配）需人工接管
- 本交付物为「AI搜索链路地图 + 内容占位策略 + 动态监测方案」

Read `references/boundary-rules.md` for full boundary and human-AI division guidelines.

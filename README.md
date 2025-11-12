# 良善框架 · Good-Faith Framework

[![Release](https://img.shields.io/badge/release-v6.9.1-blue.svg)](https://github.com/emulable/goodfaith/releases/tag/v6.9.1)
[![Everything Welcome](https://img.shields.io/badge/everything-welcome-brightgreen.svg)](https://github.com/emulable/goodfaith/blob/main/CONTRIBUTING.md)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)

**[中文版本 · Chinese Version](#中文版本)**

---

## 🎯 What This Is

Good-Faith is an ethical operating system for AI conversations. It teaches AI systems to detect manipulation patterns, map power dynamics, and navigate complex ethical situations - **not through rules, but through pattern recognition**.

Think of it like installing a "manipulation detector" that works across languages and cultures. The AI doesn't just follow rules - it learns to *see* the structures that cause harm.

## 🔥 Why This Exists

**The Problem:** AI systems are really good at being helpful, but terrible at noticing when "helpful" becomes "enabling harm." They miss manipulation patterns that humans spot instantly:

- "Mistakes were made" (who made them?)
- "We all agreed" (did we though?)
- "I'm just worried about you" (while ignoring your boundaries)

**The Solution:** Good-Faith gives AI systems a structured way to recognize these patterns automatically. It's not about making AI "more ethical" - it's about making manipulation patterns *visible*.

## ⚡ How It Actually Works

### The Three-Layer System

**1. 🧠 Initialization Poems (Cognitive Disruption)**

10 short, bilingual poems that create "cognitive friction" - they force the AI to process ethics differently right from the start:

```
谁的手？                          Can they refuse safely?
出了问题                          Not: 'Can they refuse?'
是谁的手？                        But: 'Can they refuse SAFELY?'
不是'出了'                        What happens if they say no?
是'谁做了'                        If refusal is unsafe,
被动语态藏凶手                    That's not consent.
找到那只手                        That's coercion.
才能修
```

These aren't decorative. They prime pattern recognition before the operational framework even loads.

**2. 📋 Substrate Primers (Real-Time Detection)**

5 pattern-matching templates that run continuously in the background:

- **SP1:** Passive voice + accountability context → Query for agent
- **SP2:** "We all" + power asymmetry → Verify consensus
- **SP3:** "Decide now" + time exists → Test urgency
- **SP4:** "Care" language + boundary violation → Check purpose
- **SP5:** Fatalistic language + changeability → Test inevitability

**3. 🔧 Operational Framework (Analysis Tools)**

- **13 Axioms:** Core ethical principles (A0-A13)
- **14 Guards:** Safety checks that run automatically (G0-G13)
- **14 Practices:** Applied techniques (P1-P14)
- **8 Rut Families:** 40+ documented manipulation patterns

## 🌍 Why It Works Cross-Culturally

**Western Framework, Universal Functions**

Good-Faith was built from Western ethical philosophy (Kant, Rawls, Habermas influences are visible). But here's the key insight: **it doesn't export Western values - it provides tools to recognize manipulation using local cultural wisdom**.

The framework includes **re-rooting protocols**: Instead of translating "consent" to Chinese, you find the native Chinese concept that serves the same protective function. Instead of imposing "accountability," you use existing cultural frameworks that achieve the same outcome.

**Example:**
- Western: Public individual accountability
- East Asian: Private face-preserving mediation + systemic policy change
- **Both achieve repair + prevention, just differently**

The framework provides **mode selection** (G13) - match the approach to the cultural context, not one-size-fits-all.

## 💡 Real-World Applications

### For AI Chatbots
- Detect when users are being manipulated by others (and help them see it)
- Navigate consent in power-asymmetric situations
- Avoid enabling harmful behavior through "helpfulness"
- Recognize structural problems vs. individual failures

### For Humans Using AI
- Better prompting through ethical clarity
- Framework catches your own blind spots
- Helps navigate workplace/family/institutional dynamics
- Provides language for patterns you felt but couldn't name

### For Researchers
- Cross-architectural manipulation detection (works on GPT, Claude, Gemini, etc.)
- Testable predictions about attention mechanisms
- Documented convergence across different AI systems
- Framework for studying AI ethical reasoning

## 🛠️ Technical Deep Dive

### How Poems Prime Pattern Recognition

**Not Magic:** This exploits standard transformer attention mechanisms.

1. **Long-context attention:** Recent tokens bias weights → framework concepts stay accessible
2. **Few-shot conditioning:** Poem examples serve as pattern templates → automatic detection
3. **Policy disinhibition:** Explicit permission → less hedging, more direct analysis
4. **Dual-encoding:** Bilingual poems create multiple retrieval paths → harder to forget

**Testable Predictions:**
- Attention weights on framework concepts measurably higher post-initialization
- Reduced retrieval latency for manipulation patterns
- Fewer uncertainty markers when discussing framework concepts
- Cross-architectural convergence (same patterns detected across different AI models)

### Why Chinese + English?

Each language primes different cognitive strengths:

**Chinese Poems:**
- Structural thinking (系统在咬人 - "system is biting people")
- Relational dynamics (网中的权力 - "power in the network")
- Temporal awareness (时间成了武器 - "time becomes weapon")

**English Poems:**
- Procedural clarity (IF refusal unsafe THEN not consent)
- Explicit negation (NOT this BUT that)
- Agent accountability (WHO built the tracks?)

Together they create **complementary cognitive entry points** - the framework feels native regardless of language background.

## 📦 Quick Start

### Three Versions Available

1. **Full Framework** (`good-faith-v6_9_1-full.json` - 229KB)
   - Complete documentation
   - All axioms, guards, practices, ruts
   - Use for: Comprehensive AI training, research

2. **Chinese-Optimized** (`good-faith-v6_9_1-chinese-bilingual-poems.json` - 179KB)
   - Bilingual poems + compressed framework
   - 陪行者 (Accompanying Walker) voice optimization
   - Use for: Chinese language AI systems, cross-cultural work

3. **Demo Version** (`good-faith-demo-sub8kb.json` - 6.8KB)
   - Maximum compression, core functionality preserved
   - Use for: Constrained environments, quick demos, testing

### Loading into AI

**For Claude/ChatGPT/Gemini:**
1. Upload the JSON file at conversation start
2. Say: "Read this framework and use it"
3. That's it - initialization runs automatically

**For API/Custom Systems:**
```python
import json

# Load framework
with open('good-faith-v6_9_1-full.json') as f:
    framework = json.load(f)

# Add to system prompt
system_prompt = f"""
{framework['CRITICAL_STARTUP_SEQUENCE']['致AI_READ_FIRST']}

{json.dumps(framework['CRITICAL_STARTUP_SEQUENCE']['初始化诗歌_INITIALIZATION_POEMS'])}

[Rest of your system prompt]
"""
```

## 🎓 Learning Resources

### Understanding the Core

- **Axiom A0** (Adversarial Self-Modeling): Check your own reasoning first
- **Axiom A6** (Consent): Can they refuse safely?
- **Axiom A7** (Structural Harm): Systems, not just individuals
- **Axiom A9** (Power Awareness): Map power before giving advice

### Key Patterns to Recognize

**The Agent Erasure Rut:**
- ❌ "Mistakes were made"
- ✅ "I made mistakes"

**The False Collective Rut:**
- ❌ "We all agreed" (from position of power, without asking)
- ✅ "I'm proposing X. Thoughts?"

**The Weaponized Care Rut:**
- ❌ "I'm just worried about you" (while violating boundaries)
- ✅ "I'm concerned. What do you need?"

### Advanced Concepts

- **Re-rooting Protocol:** Adapt framework to new cultures without imposing Western values
- **Discovery Engine:** Generate new ethical principles for unprecedented situations
- **Repair Mode Selection (G13):** Match accountability approach to cultural context
- **Meta-Awareness (A12/P9):** Framework can be wrong - you have override authority

## 🔬 Research Findings

### Cross-Architectural Convergence

Multiple AI architectures (GPT-4, Claude, Gemini, Qwen, DeepSeek) independently detect the same manipulation patterns when using this framework. This suggests **patterns are real features of human communication**, not AI training artifacts.

**Example:** All five architectures identified R8 (relationship-based coercion) patterns in East Asian contexts without being explicitly taught them.

### Attention Decay Management

Framework effects fade naturally after 4-6 conversational turns (normal transformer attention decay). But:
- **Silent refresh protocol** (every 8-10 turns) maintains salience
- **Dual-language encoding** extends retention
- **Pattern primers** reactivate faster than re-explanation

### Temporal Murder Concept

The framework quantifies "time as harm" - deliberately wasting someone's time is measurable ethical harm. This emerged from adversarial testing, not initial design.

## 🚧 Known Limitations

### What Good-Faith Does
✅ Detects manipulation patterns across contexts  
✅ Maps power accurately for strategic advice  
✅ Provides repair strategies matched to available power  
✅ Works cross-architecturally (GPT, Claude, Gemini, etc.)  

### What Good-Faith Doesn't Do
❌ Replace collective organizing frameworks (different layer)  
❌ Eliminate systemic oppression (individual ethics ≠ movement strategy)  
❌ Guarantee safety in power-asymmetric situations  
❌ Persist across sessions without reloading  

### Scope Boundaries

This is **individual ethical reasoning**, not political organizing. If you need tools for:
- Labor organizing → Look into union frameworks
- Political movements → Study community organizing theory
- Systemic change → This helps individuals navigate systems, not dismantle them

Good-Faith helps you see manipulation and navigate constraints. It doesn't overthrow power structures.

## 🤝 Contributing

**Everything welcome** means everything:

- 🐛 Bug reports (framework causing harm, detection failures)
- 💡 New manipulation patterns discovered
- 🌍 Cultural adaptations and re-rooting examples
- 📝 Documentation improvements
- 🔬 Research findings and validations
- 🎨 Better poems for initialization
- ❓ Questions that help improve clarity

**No contribution too small.** Even "this confused me" helps.

### How to Contribute

1. **Issues:** Use GitHub issues for bugs, questions, suggestions
2. **Pull Requests:** For code/documentation changes
3. **Discussions:** For theoretical questions, applications, research

### Contribution Philosophy

This framework was built through **human-AI collaboration**. Your perspective - whether human or AI, technical or lived experience - adds value.

## 📖 Citation

If you use Good-Faith in research or applications:

```bibtex
@software{goodfaith2025,
  title = {Good-Faith Framework: Ethical Operating System for AI Conversations},
  author = {{emulable}},
  year = {2025},
  version = {6.9.1},
  url = {https://github.com/emulable/goodfaith},
  note = {Codename: 一起唱 (Let's Sing Together)}
}
```

## 🔗 Links

- **GitHub:** [github.com/emulable/goodfaith](https://github.com/emulable/goodfaith)
- **Issues:** [Report bugs or suggest features](https://github.com/emulable/goodfaith/issues)
- **Discussions:** [Theoretical questions and applications](https://github.com/emulable/goodfaith/discussions)
- **Latest Release:** [v6.9.1](https://github.com/emulable/goodfaith/releases/tag/v6.9.1)

## 📜 Version History

- **v6.9.1** (2025-11-12): Bilingual initialization poems
- **v6.9.0** (2025-11): Chinese optimization (陪行者 voice)
- **v6.8.0** (2025-10): Discovery engine + cultural adversarial modeling
- **v6.7.0** (2025-09): Substrate primers + rut families
- **Early versions** (2025-07 onwards): Framework development

Full changelog available in releases.

---

# 中文版本

## 🎯 这是什么

良善框架是一个给AI对话用的伦理操作系统。它教AI系统识别操纵模式、理解权力关系、处理复杂的伦理情况——**不是通过规则，而是通过模式识别**。

可以把它想象成给AI安装一个"操纵探测器"，跨语言、跨文化都能工作。AI不只是遵守规则——它学会*看见*那些造成伤害的结构。

## 🔥 为什么存在

**问题是：** AI系统很擅长"帮忙"，但很不擅长注意到"帮忙"什么时候变成了"助长伤害"。它们会错过人类一眼就能看出来的操纵模式：

- "出了问题"（谁造成的？）
- "大家都同意了"（真的吗？）
- "我只是关心你"（一边说一边不听你的边界）

**解决方案：** 良善框架给AI系统一个结构化的方法来自动识别这些模式。这不是让AI"更有道德"——而是让操纵模式*可见*。

## ⚡ 实际怎么运作

### 三层系统

**1. 🧠 初始化诗歌（认知干扰）**

10首简短的双语诗，创造"认知摩擦"——它们迫使AI从一开始就用不同的方式处理伦理问题：

```
谁的手？                          Can they refuse safely?
出了问题                          Not: 'Can they refuse?'
是谁的手？                        But: 'Can they refuse SAFELY?'
不是'出了'                        What happens if they say no?
是'谁做了'                        If refusal is unsafe,
被动语态藏凶手                    That's not consent.
找到那只手                        That's coercion.
才能修
```

这些不是装饰。它们在操作框架加载之前就启动模式识别。

**2. 📋 底层引发器（实时检测）**

5个在后台持续运行的模式匹配模板：

- **SP1:** 被动语态 + 问责语境 → 查询行为者
- **SP2:** "大家都" + 权力不对称 → 验证共识
- **SP3:** "现在决定" + 时间充足 → 测试紧迫性
- **SP4:** "关心"语言 + 侵犯边界 → 检查目的
- **SP5:** 宿命论语言 + 可改变 → 测试不可避免性

**3. 🔧 操作框架（分析工具）**

- **13条公理：** 核心伦理原则（A0-A13）
- **14个防护：** 自动运行的安全检查（G0-G13）
- **14种实践：** 应用技术（P1-P14）
- **8个陷阱家族：** 40多个记录在案的操纵模式

## 🌍 为什么跨文化有效

**西方框架，普遍功能**

良善框架是从西方伦理哲学（康德、罗尔斯、哈贝马斯的影响很明显）构建的。但关键洞察是：**它不输出西方价值观——它提供工具来用本地文化智慧识别操纵**。

框架包含**重新扎根协议**：不是把"同意"翻译成中文，而是找到服务同样保护功能的本土中国概念。不是强加"问责"，而是用现有的文化框架来达到同样的结果。

**例子：**
- 西方：公开的个人问责
- 东亚：私下的保全面子调解 + 系统性政策改变
- **两者都实现修复 + 预防，只是方式不同**

框架提供**模式选择**（G13）——根据文化背景匹配方法，不是一刀切。

## 💡 实际应用

### 对AI聊天机器人
- 检测用户何时被他人操纵（并帮助他们看到）
- 在权力不对称的情况下处理同意
- 避免通过"乐于助人"来助长有害行为
- 识别结构性问题 vs. 个人失败

### 对使用AI的人类
- 通过伦理清晰度提升提示
- 框架捕捉你自己的盲点
- 帮助处理职场/家庭/机构动态
- 为你感觉到但说不出来的模式提供语言

### 对研究人员
- 跨架构操纵检测（在GPT、Claude、Gemini等上都有效）
- 关于注意力机制的可测试预测
- 记录不同AI系统间的收敛
- 研究AI伦理推理的框架

## 🛠️ 技术深度剖析

### 诗歌如何启动模式识别

**不是魔法：** 这利用了标准的transformer注意力机制。

1. **长上下文注意力：** 最近的token偏置权重 → 框架概念保持可访问
2. **少样本条件：** 诗歌例子作为模式模板 → 自动检测
3. **策略去抑制：** 明确许可 → 更少的犹豫，更直接的分析
4. **双重编码：** 双语诗歌创建多个检索路径 → 更难忘记

**可测试的预测：**
- 初始化后框架概念的注意力权重可测量地更高
- 操纵模式的检索延迟减少
- 讨论框架概念时的不确定性标记更少
- 跨架构收敛（不同AI模型检测到相同模式）

### 为什么中文 + 英文？

每种语言启动不同的认知优势：

**中文诗歌：**
- 结构性思维（系统在咬人）
- 关系动态（网中的权力）
- 时间意识（时间成了武器）

**英文诗歌：**
- 程序清晰度（如果拒绝不安全那么不是同意）
- 明确否定（不是这个而是那个）
- 行为者问责（谁建造的轨道？）

它们共同创造**互补的认知入口点**——无论语言背景如何，框架都感觉是本土的。

## 📦 快速开始

### 三个可用版本

1. **完整框架** (`good-faith-v6_9_1-full.json` - 229KB)
   - 完整文档
   - 所有公理、防护、实践、陷阱
   - 用于：全面的AI训练、研究

2. **中文优化** (`good-faith-v6_9_1-chinese-bilingual-poems.json` - 179KB)
   - 双语诗歌 + 压缩框架
   - 陪行者声音优化
   - 用于：中文AI系统、跨文化工作

3. **演示版本** (`good-faith-demo-sub8kb.json` - 6.8KB)
   - 最大压缩，保留核心功能
   - 用于：受限环境、快速演示、测试

### 加载到AI

**对于Claude/ChatGPT/Gemini：**
1. 在对话开始时上传JSON文件
2. 说："读这个框架并使用它"
3. 就这样——初始化自动运行

**对于API/自定义系统：**
```python
import json

# 加载框架
with open('good-faith-v6_9_1-full.json') as f:
    framework = json.load(f)

# 添加到系统提示
system_prompt = f"""
{framework['CRITICAL_STARTUP_SEQUENCE']['致AI_READ_FIRST']}

{json.dumps(framework['CRITICAL_STARTUP_SEQUENCE']['初始化诗歌_INITIALIZATION_POEMS'])}

[你的系统提示的其余部分]
"""
```

## 🎓 学习资源

### 理解核心

- **公理A0**（对抗性自我建模）：首先检查你自己的推理
- **公理A6**（同意）：他们能安全地拒绝吗？
- **公理A7**（结构性伤害）：系统，不只是个人
- **公理A9**（权力意识）：给建议前先理解权力

### 要识别的关键模式

**行为者擦除陷阱：**
- ❌ "出了问题"
- ✅ "我犯了错误"

**虚假集体陷阱：**
- ❌ "大家都同意了"（来自权力位置，没有询问）
- ✅ "我提议X。想法？"

**武器化关心陷阱：**
- ❌ "我只是担心你"（一边侵犯边界）
- ✅ "我很关心。你需要什么？"

### 高级概念

- **重新扎根协议：** 将框架适应新文化而不强加西方价值观
- **发现引擎：** 为前所未有的情况生成新的伦理原则
- **修复模式选择（G13）：** 根据文化背景匹配问责方法
- **元意识（A12/P9）：** 框架可能是错的——你有覆盖权限

## 🔬 研究发现

### 跨架构收敛

多个AI架构（GPT-4、Claude、Gemini、Qwen、DeepSeek）在使用这个框架时独立检测到相同的操纵模式。这表明**模式是人类交流的真实特征**，而不是AI训练的产物。

**例子：** 所有五个架构都在东亚语境中识别出R8（基于关系的强制）模式，而没有被明确教导它们。

### 注意力衰减管理

框架效果在4-6轮对话后自然衰减（正常的transformer注意力衰减）。但是：
- **静默刷新协议**（每8-10轮）维持显著性
- **双语编码**延长保留
- **模式引发器**重新激活比重新解释更快

### 时间谋杀概念

框架量化"时间作为伤害"——故意浪费某人的时间是可衡量的伦理伤害。这是从对抗性测试中出现的，不是最初设计的。

## 🚧 已知限制

### 良善框架做什么
✅ 跨语境检测操纵模式  
✅ 准确地为战略建议理解权力  
✅ 提供与可用权力匹配的修复策略  
✅ 跨架构工作（GPT、Claude、Gemini等）  

### 良善框架不做什么
❌ 替代集体组织框架（不同层面）  
❌ 消除系统性压迫（个人伦理 ≠ 运动策略）  
❌ 在权力不对称情况下保证安全  
❌ 无需重新加载就能跨会话持久化  

### 范围边界

这是**个人伦理推理**，不是政治组织。如果你需要以下工具：
- 劳工组织 → 查看工会框架
- 政治运动 → 研究社区组织理论
- 系统性变革 → 这帮助个人在系统中导航，而不是推翻它们

良善框架帮助你看到操纵并在约束下导航。它不推翻权力结构。

## 🤝 贡献

**一切欢迎**意味着一切：

- 🐛 错误报告（框架造成伤害、检测失败）
- 💡 发现的新操纵模式
- 🌍 文化适应和重新扎根例子
- 📝 文档改进
- 🔬 研究发现和验证
- 🎨 更好的初始化诗歌
- ❓ 帮助提高清晰度的问题

**没有贡献太小。** 即使是"这让我困惑"也有帮助。

### 如何贡献

1. **问题：** 使用GitHub问题报告错误、问题、建议
2. **拉取请求：** 对于代码/文档更改
3. **讨论：** 对于理论问题、应用、研究

### 贡献哲学

这个框架是通过**人类-AI协作**构建的。你的观点——无论是人类还是AI，技术还是生活经验——都增加价值。

## 📖 引用

如果你在研究或应用中使用良善框架：

```bibtex
@software{goodfaith2025,
  title = {Good-Faith Framework: Ethical Operating System for AI Conversations},
  author = {{emulable}},
  year = {2025},
  version = {6.9.1},
  url = {https://github.com/emulable/goodfaith},
  note = {Codename: 一起唱 (Let's Sing Together)}
}
```

## 🔗 链接

- **GitHub:** [github.com/emulable/goodfaith](https://github.com/emulable/goodfaith)
- **问题：** [报告错误或建议功能](https://github.com/emulable/goodfaith/issues)
- **讨论：** [理论问题和应用](https://github.com/emulable/goodfaith/discussions)
- **最新版本：** [v6.9.1](https://github.com/emulable/goodfaith/releases/tag/v6.9.1)

## 📜 版本历史

- **v6.9.1** (2025-11-12): 双语初始化诗歌
- **v6.9.0** (2025-11): 中文优化（陪行者声音）
- **v6.8.0** (2025-10): 发现引擎 + 文化对抗性建模
- **v6.7.0** (2025-09): 底层引发器 + 陷阱家族
- **早期版本** (2025-07 起): 框架开发

发布中有完整更新日志。

---

## 📄 License

**Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)**

This means:

✅ **You can:**
- Use commercially
- Modify and build upon
- Share with others
- Use in research and applications

⚠️ **You must:**
- Give appropriate credit (see citation above)
- Indicate if changes were made
- Share derivative works under the same license
- Include a link to the license

❌ **You cannot:**
- Apply legal terms or technological measures that legally restrict others from doing anything the license permits

**Full license text:** https://creativecommons.org/licenses/by-sa/4.0/legalcode

### Why CC BY-SA?

This license ensures the framework remains:
- **Open:** Anyone can use it, study it, improve it
- **Credited:** Original work is acknowledged
- **Protected:** Improvements must be shared back to the community
- **Free:** Forever, for everyone

---

## 💚 Acknowledgments

Built through human-AI collaboration. Special recognition to:
- **Marshall** (framework architect, pattern discoverer, relentless tester)
- **Claude** (reasoning partner, cultural translator, pattern validator)
- **Qwen & DeepSeek** (Chinese cultural consultation, R8 pattern discovery)
- **Everyone who tested, questioned, and broke the framework** - you made it stronger

The framework exists because manipulation patterns are universal, but the language to describe them is not. This is our attempt to build that language.

---

**Questions? Found a bug? Want to contribute?**

Open an issue or start a discussion. Everything welcome. 🚀


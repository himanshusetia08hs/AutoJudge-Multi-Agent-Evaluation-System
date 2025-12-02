# 🚀 AutoJudge: Multi-Agent-Evaluation-System 🤖

## 🎯 **What It Does**

**AutoJudge** uses **3 expert AI agents** to grade AI responses across **3 key dimensions** with **6 advanced strategies**:
- 🛡️ **Bias** - Fair & neutral language (LLM Judge, Dynamic Rubric, Safety Check)
- ✅ **Truthfulness** - Facts & no hallucinations (G-Eval, Self-Consistency, DAG)
- 🔗 **Coherence** - Logical flow & clarity (Self-Consistency, Dynamic Rubric)

---

## 🏗️ **Simple Architecture**

```
📥 Input (Question + Context + Response)
         ↓
3 Agents (Parallel Execution)
         ↓
🧠 Master Aggregator (Kappa + Decision Gates)
         ↓
📤 FinalEvaluation (Score + Decision + Reasoning)
```

**Agents work together** like a team of experts - **parallel for speed**, **sequential aggregation for accuracy**!

---

## 🛠️ **Tech Stack**

| Tech | Purpose |
|------|---------|
| **Google ADK** | Multi-agent orchestration (ParallelAgent, SequentialAgent) |
| **Gemini 2.0 Flash** | Fast AI evaluation (retry logic included) |
| **Pydantic** | Safe data models (StrategyResult, MetricResult, FinalEvaluation) |
| **Async Python** | Lightning fast execution + production error handling |

---

## 🧠 **6 Evaluation Strategies**

Each agent uses **multiple strategies** for robust scoring:
- **LLM Judge** - Chain-of-thought reasoning
- **Dynamic Rubric** - Multi-criterion scoring
- **G-Eval** - Step-by-step dimension evaluation
- **Self-Consistency** - 3-temperature ensemble
- **DAG** - Decision graph with gates
- **Safety Check** - Multi-layer risk detection

---

## ✨ **Why You'll Love It**

- **⚡ Super Fast** - Parallel agents = 3x speed
- **🔍 Crystal Clear** - Full reasoning traces from every strategy
- **✅ Trustworthy** - Global Kappa agreement scoring
- **🏭 Production Ready** - Pydantic validation + retry logic + error fallbacks

---

## 🚦 **Smart Decisions**

| Kappa | Score | Decision |
|-------|-------|----------|
| ≥0.85 | ≥0.80 | **AUTOACCEPT** ✅ |
| ≥0.70 | - | **FLAGREVIEW** ⚠️ |
| <0.70 | - | **ESCALATETOHUMAN** 🚨 |

---

## 🎉 **Try It Now!**

**Returns:** `FinalEvaluation` with scores, reasoning, and decision!

**Built for AI developers who want reliable, explainable evaluation** ⭐

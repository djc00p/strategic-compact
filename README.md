# 🗜️ Strategic Compact

[![ClawHub Skill](https://img.shields.io/badge/ClawHub-Skill-blue)](https://clawhub.ai/djc00p/strategic-compact) [![Agent Skill](https://img.shields.io/badge/Agent-Skill-blue)](#) [![Context](https://img.shields.io/badge/Context-Management-FF6B6B.svg)](https://en.wikipedia.org/wiki/Context_(computing) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**Strategic Compact** teaches manual `/compact` at *logical workflow boundaries* — instead of letting auto-compaction fire at arbitrary points.

Auto-compaction is a pressure valve, not a strategy. It triggers when context fills, which is often mid-task, mid-reasoning, right after you learned something expensive. That knowledge evaporates along with the token budget. Strategic compaction puts the checkpoint **where you chose it**, right after you've written the important findings to disk.

---

## 🎯 When to Activate

* Running long sessions approaching context limits (200K+ tokens)
* Multi-phase tasks — research → plan → implement → test
* Switching between unrelated tasks within the same session
* After completing a major milestone, before starting new work

---

## 🚀 Quick Start

1. **Identify logical phase boundaries** in your work
2. **Save important findings to files** before compacting
3. **Use `/compact` with a context message** — e.g. `/compact Now implementing auth`
4. **Continue work referencing saved files**, not conversation history

---

## 🧠 The Problem With Auto-Compaction

| Auto-compaction | Strategic compaction |
|-----------------|---------------------|
| Fires at arbitrary token thresholds | Fires at phase boundaries you chose |
| Often lands mid-task | Lands after exploration/planning, before execution |
| Discards reasoning you still need | Reasoning was already written to files |
| You don't control the summary | You supply the context message |

---

## 📦 What Survives Compaction

**Survives:** project instructions, git state, files on disk

**Does not survive:** conversation history, intermediate reasoning

That asymmetry is the whole reason for checkpoint discipline: **anything you might need after compaction must be in a file before you compact.**

---

## 🎯 Token Awareness

| Context | Action |
|---------|--------|
| **150K** | Consider compacting |
| **180K** | Plan the compaction |
| **200K+** | Should have already compacted |

---

## 📋 Common Compaction Points

* **Research → build** — compact after the documentation phase
* **Exploration → execution** — compact after `CLAUDE.md` is written
* **Debug → next feature** — compact after the fix is committed
* **Failed approach → new strategy** — compact to clear dead-end reasoning

---

## 🧭 Checkpoint Discipline

* Save learnings to files — don't rely on the transcript
* Use git commits to mark progress — the commit message is durable context
* Name the phase in the `/compact` message so the next turn starts oriented

---

## 📚 References

* `references/compaction-strategy.md` — when to compact, what to write first
* `references/checkpoint-patterns.md` — file-based persistence patterns

---

**Published by [@djc00p](https://github.com/djc00p)**

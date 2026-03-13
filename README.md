# Agentic Code Reviewer 🤖💻

An autonomous AI Agent designed to analyze repository structures, perform deep code reviews, and suggest refactoring patterns to improve maintainability and security.

## 🧠 The Agentic Approach

Unlike static analysis tools, this agent uses a **ReAct (Reasoning + Acting)** loop to:
1. **Map:** Understand file dependencies and architectural patterns.
2. **Analyze:** Identify code smells, security vulnerabilities, and performance bottlenecks.
3. **Propose:** Generate precise diffs for refactoring.
4. **Verify:** (Optional) Run existing tests to ensure the proposed changes are safe.

## 🚀 Features

- **Context-Aware Reviews:** Understands the broader context of your codebase, not just individual files.
- **Customizable Guidelines:** Define your own coding standards via a `policy.yaml` file.
- **GitHub Integration:** Automatically comments on Pull Requests with constructive feedback.
- **Refactoring Proposals:** Beyond just identifying issues, it provides production-ready code fixes.

## 🛠️ Tech Stack

- **Framework:** LangChain / AutoGPT.
- **Models:** GPT-4-turbo, Claude-3.5-Sonnet.
- **Analysis:** Tree-sitter for AST parsing.

## 📦 Installation

```bash
pip install -r requirements.txt
python agent.py --repo_path ./my-project
```
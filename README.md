# AIR – Artificial Intelligence Resident

<p align="center">
  <em>Fully offline AI assistant for your terminal.</em>
</p>

---

## About the project

AIR is a command-line tool that brings a powerful AI assistant directly into your terminal.  
It works **completely offline**, using local language models through [Ollama](https://ollama.com).

The project is a fork of the excellent [Aider](https://github.com/paul-gauthier/aider), rebuilt for those who care about privacy and want full control over their tools.

---

## Why AIR

- **No internet required** – everything runs locally on your machine.
- **Local models** – uses Ollama to run Qwen 2.5, Llama 3, DeepSeek and many other open models.
- **Terminal-first** – chat with the AI just like you would with a colleague in the command line.
- **Real tools** – the agent can read, edit and write files, execute shell commands, work with Git, perform calculations and more.
- **Open source** – licensed under Apache 2.0, free to modify and distribute.

---

## What AIR can do

- **Write and refactor code** – works with Python, JavaScript, Rust, Go, C++, Ruby and dozens of other languages.
- **Automate terminal tasks** – run commands and get explanations in the same session.
- **Manage Git repositories** – automatically create meaningful commits for AI-made changes.
- **Handle files** – create, read and modify any text-based file on your system.
- **Solve math and logic problems** – from simple arithmetic to complex formulas.
- **Understand your codebase** – builds a map of your project and uses it to give context-aware answers.
- **Communicate in multiple languages** – English, Russian, and many others are supported.

AIR is designed for developers who want a capable, independent AI assistant without monthly fees or cloud dependencies.

---

## Installation

### Prerequisites

- **Python 3.10** or newer
- **Ollama** – installation instructions at [ollama.com](https://ollama.com)

After installing Ollama, download a lightweight model:

```bash
ollama pull qwen2.5:7b-q4_K_M

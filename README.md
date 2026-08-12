# AIR – Artificial Intelligence Resident

*Fully offline AI assistant for your terminal.*

---

## About

AIR is a command-line tool that brings a powerful AI assistant directly into your terminal.  
It works **completely offline**, using local language models through [Ollama](https://ollama.com).


---

## What AIR Can Do

- Write and refactor code (Python, JS, Rust, Go, C++, Ruby, and many others)
- Execute terminal commands and explain their output
- Automatically create meaningful Git commits for AI-made changes
- Read, create, and edit any text file on your system
- Solve math and logic problems, from arithmetic to complex formulas
- Build a map of your codebase and give context-aware answers
- Communicate in English, Russian, and other languages

AIR is designed for developers who want a capable, independent AI assistant without monthly fees or cloud dependencies.

---

## Installation




### 1. Install Ollama
```bash
curl -fsSL https://ollama.com/install.sh | sh

```
Download a lightweight model
```bash

ollama pull qwen2.5:7b
```
Clone the AIR repository
``` bash

git clone https://github.com/snietOFF/AIR-Artificial-Intelligence-Resident.git

```
Install AIR using pipx
```bash

pipx ensurepath
source ~/.bashrc
pipx install git+https://github.com/snietOFF/AIR-Artificial-Intelligence-Resident.git
```
Launch AIR
```bash

air --model ollama/qwen2.5:7b
```
You will enter interactive mode and can start typing requests.

---


Default Configuration (Optional)

To avoid specifying the model every time, create a file ~/.air.conf.yml with the following content:
```yaml

model: ollama/qwen2.5:7b
check-update: false
show-model-warnings: false
```
Now the ```air``` command will automatically use this model.


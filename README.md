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

## Built-in Commands

AIR includes many slash commands for controlling the assistant and managing files:

| Command | Description |
|----------|-----------|
| `/add` | Add files to the chat so AIR can edit or review them |
| `/architect` | Enter architect/editor mode using two different models |
| `/ask` | Ask questions about the codebase without editing any files |
| `/chat-mode` | Switch to a new chat mode |
| `/clear` | Clear the chat history |
| `/code` | Ask for changes to your code |
| `/commit` | Commit edits to the repo made outside the chat |
| `/context` | Enter context mode to see surrounding code |
| `/copy` | Copy the last assistant message to the clipboard |
| `/copy-context` | Copy the current chat context as Markdown |
| `/diff` | Display the diff of changes since the last message |
| `/drop` | Remove files from the chat session to free up context |
| `/edit` / `/editor` | Open an editor to write a prompt |
| `/editor-model` | Switch the editor model to a new LLM |
| `/exit` / `/quit` | Exit the application |
| `/git` | Run a git command (output excluded from chat) |
| `/help` | Ask questions about AIR |
| `/lint` | Lint and fix files in the chat or all dirty files |
| `/load` | Load and execute commands from a file |
| `/ls` | List known files and indicate which are in the chat |
| `/map` | Print the current repository map |
| `/map-refresh` | Force a refresh of the repository map |
| `/model` | Switch the main model to a new LLM |
| `/models` | Search the list of available models |
| `/multiline-mode` | Toggle multiline mode (changes behavior of Enter and Meta+Enter) |
| `/ok` | Alias for `/code Ok, please go ahead and make those changes.` |
| `/paste` | Paste image/text from the clipboard into the chat |
| `/read-only` | Add files for reference only, or make added files read-only |
| `/reasoning-effort` | Set the reasoning effort level (number or low/medium/high) |
| `/report` | Report a problem by opening a GitHub Issue |
| `/reset` | Drop all files and clear the chat history |
| `/run` (or `!`) | Run a shell command and optionally add output to the chat |
| `/save` | Save commands to a file that can reconstruct the session |
| `/settings` | Print the current settings |
| `/test` | Run a shell command and add output to the chat on non-zero exit |
| `/think-tokens` | Set the thinking token budget (e.g., 8096, 8k, 10.5k, 0.5M) |
| `/tokens` | Report on tokens used by the current chat context |
| `/undo` | Undo the last git commit if it was done by AIR |
| `/voice` | Record and transcribe voice input |
| `/weak-model` | Switch the weak model to a new LLM |
| `/web` | Scrape a webpage, convert to Markdown, and send in a message |

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







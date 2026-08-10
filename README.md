# AIR – Artificial Intelligence Resident

<p align="center">
  <em>Fully offline AI assistant for your terminal.</em>
</p>

---

## About the project

AIR is a command-line tool that brings a powerful AI assistant directly into your terminal. It works completely offline, using local language models through Ollama. The project is a fork of the excellent Aider, rebuilt for those who care about privacy and want full control over their tools.

---

## Why AIR

- No internet required – everything runs locally on your machine.
- Local models – uses Ollama to run Qwen 2.5, Llama 3, DeepSeek and many other open models.
- Terminal-first – chat with the AI just like you would with a colleague in the command line.
- Real tools – the agent can read, edit and write files, execute shell commands, work with Git, perform calculations and more.
- Open source – licensed under Apache 2.0, free to modify and distribute.

---

## What AIR can do

- Write and refactor code – works with Python, JavaScript, Rust, Go, C++, Ruby and dozens of other languages.
- Automate terminal tasks – run commands and get explanations in the same session.
- Manage Git repositories – automatically create meaningful commits for AI-made changes.
- Handle files – create, read and modify any text-based file on your system.
- Solve math and logic problems – from simple arithmetic to complex formulas.
- Understand your codebase – builds a map of your project and uses it to give context-aware answers.
- Communicate in multiple languages – English, Russian, and many others are supported.

AIR is designed for developers who want a capable, independent AI assistant without monthly fees or cloud dependencies.

---

## Installation

First, make sure you have Python 3.10 or newer. Install Ollama from https://ollama.com, then pull a lightweight model with:

ollama pull qwen2.5:7b-q4_K_M

To get AIR, clone the repository and install it in a virtual environment:

git clone https://github.com/snietOFF/AIR-Artificial-Intelligence-Resident.git
cd AIR-Artificial-Intelligence-Resident
python3 -m venv venv
source venv/bin/activate
pip install -e .

If you prefer pipx (once the package is published on PyPI), you can use:

pipx install air-chat

or directly from the repo:

pipx install git+https://github.com/snietOFF/AIR-Artificial-Intelligence-Resident.git

After installation, launch AIR with a local model:

air --model ollama/qwen2.5:7b-q4_K_M

To avoid typing the model name each time, create a configuration file at ~/.air.conf.yml with these lines:

model: ollama/qwen2.5:7b-q4_K_M
check-update: false
show-model-warnings: false

Then just run:

air

You can customize other settings like map-refresh, auto-commits, pretty, and no-git through that same configuration file.

---

## Configuration

All settings are stored in ~/.air.conf.yml. The most useful ones are:

model: sets your default language model
map-refresh: auto or manual, controls when the repository map updates
auto-commits: enables or disables automatic Git commits
pretty: toggles colored output
no-git: allows running AIR without a Git repository

---

## Building your own version

AIR is licensed under the Apache License 2.0. You are free to modify, extend and distribute the software as your own product, as long as you retain the original copyright notice and indicate the changes you made.

---

## Credits

AIR is built on top of the amazing work by Paul Gauthier and the Aider community. Original project: https://github.com/paul-gauthier/aider

---

## Contributing

Contributions are welcome. Feel free to open an issue or submit a pull request on GitHub.

---

## License

See LICENSE.txt for the full text of the Apache 2.0 license.

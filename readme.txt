⚡ GcoreX AI — Getting Started

A modular, local-first AI assistant powered by Ollama + LLMs
Built for developers who want control, speed, and offline capability.

🚀 Features
🧠 Local LLM support (Mistral, LLaMA, Gemma, etc.)
🧩 Modular tool system (tools/ auto-loader)
🗣️ Voice input & text-to-speech
🌐 Browser + Terminal support
⚡ Offline-ready AI assistant
🛠️ Extendable with custom commands
📦 Prerequisites

Make sure your system is ready:

1. Python
Version: 3.10 or higher

Check:

python3 --version
2. Ollama (Required)

Install Ollama to run local AI models:

👉 https://ollama.com/download

After installation, pull the default model:

ollama pull mistral

💡 You can also use:

llama3
gemma
phi
⚙️ Installation
🔹 Option 1: Auto Setup (Recommended for Linux)
cd GcoreX-AI
chmod +x install_deps.sh
./install_deps.sh

✔ Installs:

System dependencies
Python packages
🔹 Option 2: Manual Setup (Any OS)
cd GcoreX-AI
pip install -r requirements.txt
▶️ Run GcoreX

Start the AI assistant:

python3 GcoreX.py

or

python GcoreX.py
🧠 How It Works
🔍 Scans tools/ directory automatically
⚙️ Loads available modules dynamically
🤖 Connects to Ollama backend
💬 Handles chat, commands, and automation
⚠️ Important Notes
🟢 Ollama must be installed and running
🧠 Model (mistral) will auto-load if not active
🎤 Ensure microphone works (for voice features)
🔊 Audio output required for TTS
🧪 Quick Test

After running, try:

hello
/calc 5+5
/speak Hello bro!
📁 Project Structure
GcoreX-AI/
│
├── 📁 core/                # 🧠 Brain of the system (LLM + routing)
│   ├── brain_router.py
│   ├── llm_engine.py
│   ├── reasoning_engine.py
│   └── memory_manager.py
│
├── 📁 tools/               # 🧩 Modular tools (auto-loaded)
│   ├── calc.py
│   ├── open_url.py
│   ├── analyze_code.py
│   └── ...
│
├── 📁 interfaces/          # 🖥️ User interfaces
│   ├── cli.py              # Terminal interface
│   ├── gui.py              # GUI (Tkinter / PyQt)
│   └── web_ui.py           # Gradio / Browser UI
│
├── 📁 voice/               # 🎤 Voice system
│   ├── tts.py              # Text-to-speech
│   ├── stt.py              # Speech-to-text
│   └── voice_manager.py
│
├── 📁 memory/              # 💾 Persistent memory
│   ├── short_term.json
│   ├── long_term.json
│   └── learning_memory.json
│
├── 📁 config/              # ⚙️ Configurations
│   ├── settings.py
│   └── constants.py
│
├── 📁 utils/               # 🔧 Helper utilities
│   ├── logger.py
│   ├── file_utils.py
│   └── helpers.py
│
├── 📁 models/              # 🤖 Model configs (Ollama)
│   ├── model_manager.py
│   └── model_config.json
│
├── 📁 tests/               # 🧪 Testing
│   └── test_tools.py
│
├── 📁 scripts/             # ⚡ Automation scripts
│   ├── install_deps.sh
│   └── setup.py
│
├── 📁 assets/              # 🎨 Static files (icons, UI)
│
├── 📁 build/               # 📦 Build files
├── 📁 dist/                # 🚀 Executables (.exe / apk)
│
├── main.py                # 🚀 Entry point (NEW)
├── requirements.txt
├── README.md
└── LICENSE.txt

Want to extend GcoreX?

Add new tools inside tools/
Follow existing module format
They will auto-load on startup ⚡
🧠 Pro Tip

If performance is slow, try lighter models:

ollama pull phi
🛠️ Troubleshooting
Issue	Fix
Ollama not detected	Run ollama serve
Model not found	ollama pull mistral
Module error	Reinstall dependencies
Mic not working	Check system permissions
💡 Future Ideas
📱 Android APK version
🖥️ Windows .exe build
🧠 Smarter model switching
🎨 Image generation
💾 Chat memory system
🤝 Contributing

Pull requests are welcome!
Add tools, improve UI, or optimize performance.

⚡ GcoreX Vision

“Your own Jarvis — fully local, fully yours.

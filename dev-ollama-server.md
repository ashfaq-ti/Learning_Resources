try: OLLAMA_HOST=127.0.0.1:9066 ollama serve

If you get a permission error, then you might need sudo: sudo OLLAMA_HOST=127.0.0.1:9066 ollama serve

or adjust permissions with: chmod +x $(which ollama)

If you’re getting ollama: command not found, it means Ollama is either not installed or not in your system's PATH.

Step 1: Check if Ollama is installed
Run:

which ollama  or  command -v ollama

use the path from above cmd in place of ollama in "sudo OLLAMA_HOST=127.0.0.1:9066 ollama serve"

sudo OLLAMA_HOST=127.0.0.1:9066 /usr/local/bin/ollama serve

sudo OLLAMA_MODELS=/usr/share/ollama/.ollama/models  OLLAMA_HOST=0.0.0.0:9066 /usr/local/bin/ollama serve

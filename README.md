# Orlun for Windows

Orlun is a thinking partner that remembers who you are: you write your own **Mind Fragments**, Orlun keeps a dated **Memory** timeline with your approval, and builds **Impressions** of how you think, all visible and correctable in your Mind Box. This is the desktop app: it runs an AI model on your own PC, so it is private, free and works offline. Gemini or Claude keys are optional.

**[Download the latest installer →](https://github.com/K3suke/Orlun/releases/latest)**

## Install

1. Download `Orlun-Setup-<version>.exe` from the latest release (about 0.7 GB).
2. Run it. This first version is **not code-signed yet**, so Windows shows "Windows protected your PC". Click **More info → Run anyway**.
3. On first launch, Orlun checks your PC (memory, graphics card, free disk) and recommends a model to download:

| Model | Download | Best for |
|---|---|---|
| Gemma 4 26B | 18.7 GB | Graphics cards with ~22 GB of memory |
| Gemma 4 12B | 8.0 GB | 8 GB+ graphics memory. What Orlun is tuned on |
| Gemma 4 E4B | 6.6 GB | Smaller graphics cards |
| Gemma 4 E2B | 4.6 GB | Modest PCs |

You can keep using Orlun while the model downloads. Already running [Ollama](https://ollama.com)? Orlun uses it and the models you have.

## Requirements

- Windows 10 or 11, 64-bit
- 16 GB of RAM recommended; an NVIDIA graphics card with 8 GB+ makes replies fast. AMD and Intel cards work through Vulkan, more slowly. Older NVIDIA cards (GTX 10-series and earlier) also run through Vulkan.
- Free disk space for the model you choose

## Privacy

Everything stays on your PC: your Mind Box, chats and the model. Nothing is sent anywhere unless you add a Gemini or Claude key, and even then local chats stay local; web searches through a key ask first and send only the search words.

## Uninstall

Settings → Apps → Orlun → Uninstall. Your data stays in `%APPDATA%\Orlun Desktop` (including downloaded models) in case you reinstall; delete that folder to remove everything.

## Licences

Orlun bundles [Ollama](https://github.com/ollama/ollama) (MIT licence; texts in `resources\licenses`). Gemma models are downloaded from Ollama's library under Google's Gemma terms (Apache 2.0 for Gemma 4).

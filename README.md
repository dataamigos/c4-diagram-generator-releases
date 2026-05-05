# C4 Diagram Generator — Releases

AI-powered desktop app that generates **draw.io XML for C4 architecture diagrams** directly inside your Miro boards — works with Gemini, Claude, and OpenAI.

---

## Download

| Version | File | Platform |
|---|---|---|
| [v1.1.0](https://github.com/dataamigos/c4-diagram-generator-releases/releases/tag/v1.1.0) | `C4DiagramGenerator.exe` | Windows 64-bit |
| [v1.0.0](https://github.com/dataamigos/c4-diagram-generator-releases/releases/tag/v1.0.0) | `C4DiagramGenerator.exe` | Windows 64-bit |

> **No installation required.** Download and double-click to run.

---

## Features

### v1.1.0 — Multi-Provider AI Support
- **Gemini** (Google) — gemini-2.0-flash, gemini-2.5-pro, gemini-1.5-flash, gemini-1.5-pro
- **Claude** (Anthropic) — claude-sonnet-4-6, claude-opus-4-7, claude-haiku-4-5
- **OpenAI** — gpt-4o, gpt-4o-mini, gpt-4-turbo, o3
- Switch providers and models from the top bar — no restart needed
- API key and settings saved per provider

### v1.0.0 — Core Features
- **Paste Miro frames directly** — right-click any Miro frame → Copy as Image → paste into the app
- **Upload image files** — PNG, JPG, BMP, WebP supported
- **Text prompt** — describe your system or request changes in plain English
- **Voice prompt** — click the mic button and speak your architecture description
- **C4 levels** — Context, Container, Component
- **Generate from scratch** — describe any system and get draw.io XML instantly
- **Update existing diagrams** — paste current XML + describe what changed → get updated XML
- **Copy to clipboard** — one click to copy XML ready to paste into draw.io
- **Save as .drawio** — save diagrams as native draw.io files

---

## How to Use

1. **Download** `C4DiagramGenerator.exe` from the latest release below
2. **Run it** — no install, no Python needed
3. **Select your AI provider** (Gemini / Claude / OpenAI) and **enter your API key** → Save
4. **From Miro:** right-click a frame → *Copy as Image* → click *Paste from Clipboard* in the app
5. **Type or speak** your prompt
6. Click **Generate** → XML appears instantly
7. In Miro: open **draw.io** add-on → **Extras → Edit Diagram** → paste XML → OK

---

## C4 Workflow with AI

```
Describe your system (text or voice)
or paste a Miro frame screenshot
            ↓
    AI generates draw.io XML
    (Gemini / Claude / OpenAI)
            ↓
  Paste into draw.io on Miro board
            ↓
  Native C4 diagram — fully editable
```

To update a diagram: paste existing XML into app, type what changed, click **Update Existing**.

---

## Requirements

- Windows 10 / 11 (64-bit)
- Internet connection (for AI API calls)
- Microphone (optional, for voice input)
- API key from one of: [Google AI Studio](https://aistudio.google.com), [Anthropic Console](https://console.anthropic.com), [OpenAI Platform](https://platform.openai.com)

---

*Source code: [dataamigos/c4-diagram-generator](https://github.com/dataamigos/c4-diagram-generator) (private)*

# C4 Diagram Generator — Releases

AI-powered desktop app that generates **draw.io XML for C4 architecture diagrams** directly inside your Miro boards — works with Gemini, Claude, and OpenAI.

---

## Download

| Version | File | Platform |
|---|---|---|
| [v1.5.1](https://github.com/dataamigos/c4-diagram-generator-releases/releases/tag/v1.5.1) | `C4DiagramGenerator.exe` | Windows 64-bit |
| [v1.5.0](https://github.com/dataamigos/c4-diagram-generator-releases/releases/tag/v1.5.0) | `C4DiagramGenerator.exe` | Windows 64-bit |
| [v1.1.0](https://github.com/dataamigos/c4-diagram-generator-releases/releases/tag/v1.1.0) | `C4DiagramGenerator.exe` | Windows 64-bit |
| [v1.0.0](https://github.com/dataamigos/c4-diagram-generator-releases/releases/tag/v1.0.0) | `C4DiagramGenerator.exe` | Windows 64-bit |

> **No installation required.** Download and double-click to run.

---

## Features

### v1.5.1 — Python Generator Mode & Token Fixes
- **🐍 Via Python checkbox** — AI writes a compact Python script (~100 tokens) that prints the XML; the app runs it locally and captures the output. No token ceiling for large C4 diagrams
- **gemini-2.5-pro** added to the model list (65 536-token output budget)
- Per-model Gemini output limits: `flash` = 8 192, `pro` / `2.5` = 65 536
- Claude raised to 16 000 tokens, OpenAI raised to 16 384 tokens
- Auto-repair of truncated XML — app closes open tags instead of crashing
- Yellow warning in status bar when a response is detected as truncated

### v1.5.0 — Official C4 Shape System
- **Exact draw.io C4 shapes** — when you say "C4 diagram" or select a C4 type, the AI uses the official `<object placeholders="1">` XML pattern with real C4 styles
- **All C4 element types**: Person (internal/external), Software System (internal/external), Container (app, database, microservice, message bus, web browser), Component
- **Nested boundaries** — System Scope Boundary and Container Scope Boundary as dashed rounded rectangles, with child elements correctly parented inside
- **Relationship arrows** use the official C4 Relationship format with technology and description labels
- **Auto-Legend** — every C4 diagram includes the standard colour-coded legend (Person, Software System, Container, Component, External Person, External Software System)
- **Smart detection** — automatically activates when prompt contains "c4 diagram", "c4 architecture", "c4 context/container/component", etc.
- **Increased token budget** — 8 192 output tokens across all providers for complex diagrams

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

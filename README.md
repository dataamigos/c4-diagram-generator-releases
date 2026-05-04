# C4 Diagram Generator — Releases

AI-powered desktop app that generates **draw.io XML for C4 architecture diagrams** directly inside your Miro boards — no tokens, no admin approval needed.

---

## Download

| Version | File | Platform |
|---|---|---|
| [v1.0.0](https://github.com/dataamigos/c4-diagram-generator-releases/releases/tag/v1.0.0) | `C4DiagramGenerator.exe` | Windows 64-bit |

> **No installation required.** Download and double-click to run.

---

## Features

### v1.0.0
- **Gemini / BlueField powered** — plug in any Gemini-compatible API key, including internal BlueField endpoints
- **Paste Miro frames directly** — right-click any Miro frame → Copy as Image → paste into the app
- **Upload image files** — PNG, JPG, BMP, WebP supported
- **Text prompt** — describe your system or request changes in plain English
- **Voice prompt** — click the mic button and speak your architecture description
- **C4 levels** — Context, Container, Component
- **Generate from scratch** — describe any system and get draw.io XML instantly
- **Update existing diagrams** — paste current XML + describe what changed → get updated XML
- **Copy to clipboard** — one click to copy XML ready to paste into draw.io
- **Save as .drawio** — save diagrams as native draw.io files
- **BlueField support** — optional custom base URL for internal LLM endpoints
- **Model selector** — gemini-2.0-flash, gemini-1.5-flash, gemini-1.5-pro, gemini-2.5-pro
- **Persistent settings** — API key and preferences saved locally between sessions

---

## How to Use

1. **Download** `C4DiagramGenerator.exe` from the latest release
2. **Run it** — no install, no Python needed
3. **Enter your API key** (Gemini or BlueField) → click Save
4. **From Miro:** right-click a frame → *Copy as Image* → click *Paste from Clipboard* in the app
5. **Type or speak** your prompt
6. Click **Generate** → XML appears
7. In Miro: open **draw.io** add-on → **Extras → Edit Diagram** → paste XML → OK

---

## C4 Workflow with AI

```
Describe your system (text or voice)
            ↓
    App calls Gemini / BlueField
            ↓
    draw.io XML generated
            ↓
  Paste into draw.io on Miro board
            ↓
  Native C4 diagram — fully editable
```

To update a diagram: paste existing XML into app, type what changed, click **Update Existing**.

---

*Source code: [dataamigos/c4-diagram-generator](https://github.com/dataamigos/c4-diagram-generator) (private)*

# 🛠️ Smart JSON Tool Pro

**Smart JSON Tool Pro** is a high-performance, browser-based utility designed for developers who deal with messy, "lazy," or slightly broken JSON. Unlike standard formatters that simply fail on syntax errors, this tool includes a **Forgiving Parser** that heals common mistakes automatically.

---

### ✨ Key Features

| Feature | Description |
| --- | --- |
| **Healing Engine** | Automatically fixes single quotes, unquoted keys, and trailing commas. |
| **Expand & Collapse** | Toggle between a beautiful 4-space indented view and a minified one-liner. |
| **Smart Search** | Real-time highlighting of keys and values within the output. |
| **File Support** | Drag and drop `.json` or `.txt` files directly into the editor. |
| **Theme Toggle** | Switch between high-contrast **Dark Mode** and clean **Light Mode**. |
| **Error Log** | Provides a detailed breakdown of exactly what was "healed" during processing. |

---

### 🚀 How to Use

1. **Input Your Data**: Paste your JSON into the left panel, or simply **drag and drop** a file from your computer.
2. **Format**: Press the **Enter** key or click **Format (Enter)**. The tool will instantly clean, heal, and prettify the code.
3. **Search**: Use the search bar to find specific data points. The tool highlights matches in real-time.
4. **Export**: Click **Copy JSON** to save the cleaned version to your clipboard instantly.

---

### ⌨️ Keyboard Shortcuts

To keep your workflow fast, the application supports the following shortcuts:

* **`Enter`**: Formats and expands the current input.
* **`Shift + Enter`**: Inserts a new line in the input area (without formatting).
* **`Ctrl/Cmd + V`**: Paste and go!

---

### 🧠 The "Healer" Logic

Standard `JSON.parse()` is very strict. This tool runs a pre-processing layer using Regular Expressions to identify and correct "Developer Laziness" before the official parse:

* **Single Quote Correction**: Converts `'key': 'value'` to `"key": "value"`.
* **Key Quoting**: Converts `{ name: "Gemini" }` to `{ "name": "Gemini" }`.
* **Comma Cleanup**: Removes trailing commas that often cause breaks in IE or strict environments.

> **Note:** While the healer is powerful, it cannot fix structural logic errors (like a missing closing bracket `}`). In those cases, the tool will provide the specific error message from the engine to help you debug.

---

### 🛠️ Installation & Deployment

This application is a **Single Page Application (SPA)**. It requires no backend, no `npm install`, and no database.

1. Clone the repository.
2. Open `index.html` in any modern web browser.
3. *(Optional)* Host it for free using **GitHub Pages**.
4. Can also view here: https://shosephiroth.github.io/JSON-Formatter/ 

---

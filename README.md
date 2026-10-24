# VoxRead — Text-to-Speech Reader

A modern, responsive text-to-speech web application built with React, TypeScript, Tailwind CSS, and the browser-native **Web Speech API** (`window.speechSynthesis`).

![VoxRead](https://img.shields.io/badge/VoxRead-Text--to--Speech-indigo)
![License](https://img.shields.io/badge/license-MIT-blue)

---

## 🚀 Features

- **Three Reading Modes**:
  - 🎓 **Study Mode**: Slower 0.85x playback cadence designed to give your working memory time to absorb complex lecture notes and technical terms.
  - 📖 **Article Mode**: Balanced 1.0x pace with dynamic reading time estimates for essays and long-form reading.
  - 🪶 **Story Mode**: Atmospheric 0.95x cadence with warm serif typography (`Lora`) and distraction-free layout.
- **Robust Speech Synthesis Engine**:
  - Automatically loads and groups all available browser voices (`speechSynthesis.onvoiceschanged`).
  - Chunks text into sentence boundaries to eliminate the common Chromium speech stall bug on long paragraphs.
  - Periodic keep-alive heartbeats for reliable long playback.
- **Interactive "Follow Along" Reader**:
  - View text broken down into sentences with real-time highlighting of the current sentence and word.
  - Click any sentence to instantly jump playback to it.
- **Complete Playback Controls**:
  - Play, Pause, Resume, and Stop controls with active status badges.
  - Speed slider (0.5x to 2.5x) with quick presets (`0.75x`, `0.85x`, `1.0x`, `1.25x`, `1.5x`, `2.0x`).
  - Voice pitch and volume sliders.
  - Keyboard shortcuts: `Space` (Play/Pause), `Escape` (Stop).
- **Editor Utilities**:
  - Character and word count display.
  - Estimated reading time calculated dynamically based on current speed.
  - Preset sample text for each mode.
  - Copy to clipboard with confirmation and Clear text action.
  - Light/Dark theme toggle with persistence.
  - Zen / Focus Mode toggle.
- **Zero Backend / Zero Paid APIs**: Runs 100% locally in your browser.

---

## 🛠️ Tech Stack

- **Framework**: [React 19](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/)
- **Bundler & Dev Server**: [Vite 6](https://vitejs.dev/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **Icons**: [Lucide React](https://lucide.dev/)
- **Audio API**: Browser-native Web Speech API (`SpeechSynthesis` & `SpeechSynthesisUtterance`)

---

## 💻 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- [npm](https://www.npmjs.com/) or [pnpm](https://pnpm.io/)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/voxread.git
   cd voxread
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the local development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to `http://localhost:5173`.

---

## 📄 License

MIT License. Feel free to use and adapt!

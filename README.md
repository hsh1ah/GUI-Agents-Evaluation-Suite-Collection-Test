# GUI-Agents-Evaluation-Suite-Collection-Test

A collection of information about HuggingFace's **GUI Agents Evaluation Suite** — [**ScreenSuite**](https://github.com/huggingface/screensuite) — focusing on desktop environment-related **Grounding benchmarks**.

---

## About ScreenSuite

[ScreenSuite](https://github.com/huggingface/screensuite) is the most comprehensive evaluation suite for GUI Agents, created by HuggingFace. It gathers and unifies **13 benchmarks** spanning the full range of GUI agent capabilities:

1. **Perception** — correctly perceiving information displayed on screen
2. **Grounding** — understanding the positioning of elements (paramount for clicking the correct place)
3. **Single-step actions** — solving instructions correctly in one action
4. **Multi-step agents** — solving higher-level goals through several actions in a GUI environment

- 📖 **Blog Post:** [huggingface.co/blog/screensuite](https://huggingface.co/blog/screensuite)
- 💻 **GitHub Repo:** [github.com/huggingface/screensuite](https://github.com/huggingface/screensuite)

---

## Desktop Environment-Related Grounding Benchmarks

These benchmarks evaluate GUI grounding (element localization / click accuracy) in **desktop computer environments** (Windows, macOS, Linux):

- **ScreenSpot**: [huggingface.co/datasets/rootsautomation/ScreenSpot](https://huggingface.co/datasets/rootsautomation/ScreenSpot)
  - The original GUI grounding benchmark covering Mobile (iOS, Android), Web, and **Desktop** (macOS, Windows, Linux).

- **ScreenSpot-Pro**: [huggingface.co/datasets/likaixin/ScreenSpot-Pro](https://huggingface.co/datasets/likaixin/ScreenSpot-Pro)
  - GUI grounding for **professional high-resolution desktop environments**. Covers 23 applications across 5 industries (Development, Creative, CAD/Engineering, Scientific/Analytical, Office Suite) and 3 operating systems (Windows, macOS, Linux).
  - Also mirrored at: [huggingface.co/datasets/HongxinLi/ScreenSpot-Pro](https://huggingface.co/datasets/HongxinLi/ScreenSpot-Pro) (used by ScreenSuite)

- **WorldGUI-Bench**: [huggingface.co/datasets/hhenryz/WorldGUI-Bench](https://huggingface.co/datasets/hhenryz/WorldGUI-Bench)
  - A dynamic desktop GUI benchmark covering 10 widely used desktop and web applications with tasks instantiated under various initial states.
  - 📄 Paper: [arxiv.org/abs/2502.08047](https://arxiv.org/abs/2502.08047)

- **OSWorld**: [github.com/xlang-ai/OSWorld](https://github.com/xlang-ai/OSWorld)
  - A multi-step agent benchmark for real computer environments (Ubuntu, Windows, macOS). Part of ScreenSuite's multi-step evaluation.

---

## Other Grounding Benchmarks in ScreenSuite

These are also part of ScreenSuite's Grounding category but focus on **Web** or **Mobile** environments:

- **ScreenSpot v2** (Web): [huggingface.co/datasets/HongxinLi/ScreenSpot_v2](https://huggingface.co/datasets/HongxinLi/ScreenSpot_v2)
- **Visual-WebBench** (Web): [huggingface.co/datasets/visualwebbench/VisualWebBench](https://huggingface.co/datasets/visualwebbench/VisualWebBench)
- **WebSRC** (Web): [huggingface.co/datasets/X-LANCE/WebSRC_v1.0](https://huggingface.co/datasets/X-LANCE/WebSRC_v1.0)
- **Showdown-Clicks** (Web): [huggingface.co/datasets/generalagents/showdown-clicks](https://huggingface.co/datasets/generalagents/showdown-clicks)
- **ScreenQA-Short** (Mobile): [huggingface.co/datasets/rootsautomation/RICO-ScreenQA-Short](https://huggingface.co/datasets/rootsautomation/RICO-ScreenQA-Short)
- **ScreenQA-Complex** (Mobile): [huggingface.co/datasets/rootsautomation/RICO-ScreenQA-Complex](https://huggingface.co/datasets/rootsautomation/RICO-ScreenQA-Complex)

---

## Quick Start

```bash
git clone --recurse-submodules git@github.com:huggingface/screensuite.git
cd screensuite
uv sync --extra submodules --python 3.11
python run.py
```

> ⚠️ Multi-step benchmarks require a bare-metal machine to run desktop/mobile environment emulators.

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

These are the **Desktop** platform benchmarks from ScreenSuite's Perception/Grounding category (as listed in the [official blog post](https://huggingface.co/blog/screensuite)):

- **ScreenSpot-v2**: [https://huggingface.co/datasets/HongxinLi/ScreenSpot_v2](https://huggingface.co/datasets/HongxinLi/ScreenSpot_v2)
- **ScreenSpot-Pro**: [https://huggingface.co/datasets/HongxinLi/ScreenSpot-Pro](https://huggingface.co/datasets/HongxinLi/ScreenSpot-Pro)

Additionally, the original **ScreenSpot** benchmark also contains desktop split data (Windows, macOS, Linux):

- **ScreenSpot**: [https://huggingface.co/datasets/rootsautomation/ScreenSpot](https://huggingface.co/datasets/rootsautomation/ScreenSpot)

---

## Desktop Multi-Step Agent Benchmark (ScreenSuite)

From ScreenSuite's Multi-Step Agents category (Desktop environment):

- **OSWorld**: Benchmarking multimodal agents for open-ended tasks in real computer environments (Ubuntu, Windows, macOS).
  - Project page: [https://os-world.github.io/](https://os-world.github.io/)
  - GitHub: [https://github.com/xlang-ai/OSWorld](https://github.com/xlang-ai/OSWorld)

---

## Other Grounding Benchmarks in ScreenSuite (Web / Mobile)

These are also part of ScreenSuite's Grounding/Perception category but focus on **Web** or **Mobile** environments:

- **Visual-WebBench** (Web): [https://huggingface.co/datasets/visualwebbench/VisualWebBench](https://huggingface.co/datasets/visualwebbench/VisualWebBench)
- **WebSRC** (Web): [https://huggingface.co/datasets/X-LANCE/WebSRC_v1.0](https://huggingface.co/datasets/X-LANCE/WebSRC_v1.0)
- **Showdown-Clicks** (Web): [https://huggingface.co/datasets/generalagents/showdown-clicks](https://huggingface.co/datasets/generalagents/showdown-clicks)
- **ScreenQA-Short** (Mobile): [https://huggingface.co/datasets/rootsautomation/RICO-ScreenQA-Short](https://huggingface.co/datasets/rootsautomation/RICO-ScreenQA-Short)
- **ScreenQA-Complex** (Mobile): [https://huggingface.co/datasets/rootsautomation/RICO-ScreenQA-Complex](https://huggingface.co/datasets/rootsautomation/RICO-ScreenQA-Complex)

---

## Quick Start

```bash
git clone --recurse-submodules git@github.com:huggingface/screensuite.git
cd screensuite
uv sync --extra submodules --python 3.11
python run.py
```

> ⚠️ Multi-step benchmarks require a bare-metal machine to run and deploy desktop/mobile environment emulators.

---

## References

- [ScreenSuite Blog Post](https://huggingface.co/blog/screensuite)
- [ScreenSuite GitHub Repository](https://github.com/huggingface/screensuite)
- [ScreenSuite on HuggingFace](https://huggingface.co/screensuite)

---
title: "Edge AI / TinyML - Collaboration Guide"
description: "Contributing guide for Edge AI / TinyML course content"
tableOfContents: true
sidebar:
  order: 999
---

# Edge AI / TinyML

![Build](https://img.shields.io/badge/build-passing-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Contributors Welcome](https://img.shields.io/badge/contributors-welcome-orange)

**Read this course at:** [https://siliconwit.com/education/edge-ai-tinyml/](https://siliconwit.com/education/edge-ai-tinyml/)

A hands-on course covering machine learning on microcontrollers. You will train, quantize, and deploy TinyML models for keyword spotting, gesture recognition, anomaly detection, image classification, and edge-cloud hybrid architectures.

## Lessons

| # | Title |
|---|-------|
| 1 | TinyML and Machine Learning on Microcontrollers |
| 2 | Edge Impulse Data Collection and Training |
| 3 | TensorFlow Lite Micro Model Deployment |
| 4 | Model Quantization and Optimization for MCUs |
| 5 | Keyword Spotting and Voice Wake Word |
| 6 | Accelerometer Gesture Recognition |
| 7 | Anomaly Detection for Predictive Maintenance |
| 8 | Camera Image Classification on ESP32 |
| 9 | Edge-Cloud Hybrid Architectures |

## File Structure

```
edge-ai-tinyml/
├── index.mdx                               # Course overview
├── tinyml-machine-learning-microcontrollers.mdx
├── edge-impulse-data-collection-training.mdx
├── tensorflow-lite-micro-model-deployment.mdx
├── model-quantization-optimization-mcu.mdx
├── keyword-spotting-voice-wake-word.mdx
├── accelerometer-gesture-recognition.mdx
├── anomaly-detection-predictive-maintenance.mdx
├── camera-image-classification-esp32.mdx
├── edge-cloud-hybrid-architecture.mdx
└── README.md
```

## How to Contribute

All commands below work on Linux, macOS, and Windows (using Git Bash, PowerShell, or Command Prompt with Git installed).

### For Team Members (with push access)

**First time setup (clone the repo once):**

```bash
git clone https://github.com/SiliconWit/edge-ai-tinyml.git
cd edge-ai-tinyml
```

**Every time you start working:**

```bash
git pull origin main
```

Always pull before making changes. This avoids conflicts with other contributors.

**After making your changes:**

```bash
git add .
git commit -m "Brief description of what you changed"
git push origin main
```

**If you get a push error** (someone pushed before you):

```bash
git pull origin main
```

Git will merge the changes automatically in most cases. If there is a conflict, Git will mark the conflicting lines in the file. Open the file, choose which version to keep, then:

```bash
git add .
git commit -m "Resolve merge conflict"
git push origin main
```

**Tips to avoid conflicts:**

- Always `git pull origin main` before you start working
- Push your changes as soon as you are done, do not hold onto uncommitted work for long
- Coordinate with other contributors so two people are not editing the same file at the same time

### For External Contributors (without push access)

1. Fork the repository: [SiliconWit/edge-ai-tinyml](https://github.com/SiliconWit/edge-ai-tinyml)
2. Clone your fork:
   ```bash
   git clone https://github.com/YOUR-USERNAME/edge-ai-tinyml.git
   cd edge-ai-tinyml
   ```
3. Make your changes and commit:
   ```bash
   git add .
   git commit -m "Brief description of what you changed"
   git push origin main
   ```
4. Open a Pull Request against `main` on the original repository
5. Describe what you changed and why in the PR description

## Content Standards

- All lesson files use `.mdx` format
- Do not use `<BionicText>` in this course
- Code blocks should include a title attribute:
  ````mdx
  ```c title="main.c"
  #include "tensorflow/lite/micro/micro_interpreter.h"
  ```
  ````
- Use Starlight components (`<Tabs>`, `<TabItem>`, `<Steps>`, `<Card>`) where appropriate
- Keep paragraphs concise and focused on practical application
- Include working code examples that readers can run directly

## Local Development

Clone the main site repository and initialize submodules:

```bash
git clone --recurse-submodules <main-repo-url>
cd siliconwit-com
npm install
npm run dev
```

To test a production build:

```bash
npm run build
```

## License

This course content is released under the [MIT License](LICENSE).

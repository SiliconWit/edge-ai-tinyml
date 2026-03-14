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

1. Fork the repository: [SiliconWit/edge-ai-tinyml](https://github.com/SiliconWit/edge-ai-tinyml)
2. Create a feature branch: `git checkout -b feature/your-topic`
3. Make your changes and commit with a clear message
4. Push to your fork and open a Pull Request against `main`
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

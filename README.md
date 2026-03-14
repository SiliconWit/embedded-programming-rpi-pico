---
title: "Embedded Programming RPi Pico - Collaboration Guide"
description: "Contributing guide for Embedded Programming RPi Pico course content"
tableOfContents: true
sidebar:
  order: 999
---

# Embedded Programming RPi Pico

![Build](https://img.shields.io/badge/build-passing-brightgreen)
![License](https://img.shields.io/badge/license-MIT-blue)
![Contributors Welcome](https://img.shields.io/badge/contributors-welcome-orange)

**Read this course at:** [https://siliconwit.com/education/embedded-programming-rpi-pico/](https://siliconwit.com/education/embedded-programming-rpi-pico/)

A course on RP2040 development using the Pico C/C++ SDK. Lessons cover PIO programmable state machines, multicore programming, DMA, USB device classes, MicroPython, and wireless connectivity with Pico W.

## Lessons

| # | Title |
|---|-------|
| 1 | Pico SDK and RP2040 Architecture |
| 2 | GPIO PWM and Analog IO |
| 3 | PIO State Machines |
| 4 | Multicore Programming |
| 5 | DMA and Data Pipelines |
| 6 | USB Device Classes |
| 7 | MicroPython on RP2040 |
| 8 | Wireless with Pico W |

## File Structure

```
embedded-programming-rpi-pico/
├── lesson-0.mdx        # Course introduction
├── lesson-1.mdx        # Pico SDK and RP2040 Architecture
├── lesson-2.mdx        # GPIO PWM and Analog IO
├── lesson-3.mdx        # PIO State Machines
├── lesson-4.mdx        # Multicore Programming
├── lesson-5.mdx        # DMA and Data Pipelines
├── lesson-6.mdx        # USB Device Classes
├── lesson-7.mdx        # MicroPython on RP2040
├── lesson-8.mdx        # Wireless with Pico W
└── README.md
```

## How to Contribute

1. Fork the repository: [SiliconWit/embedded-programming-rpi-pico](https://github.com/SiliconWit/embedded-programming-rpi-pico)
2. Create a feature branch: `git checkout -b feature/your-topic`
3. Make your changes and commit with a clear message
4. Push to your fork and open a Pull Request against `main`
5. Describe what you changed and why in the PR description

## Content Standards

- All lesson files use `.mdx` format
- Do not use `<BionicText>` in this course
- Code blocks should include a title attribute:
  ````mdx
  ```c title="blink.c"
  gpio_put(PICO_DEFAULT_LED_PIN, 1);
  ```
  ````
- Use Starlight components (`<Tabs>`, `<TabItem>`, `<Steps>`, `<Card>`) where appropriate
- Keep paragraphs concise and focused on practical application
- Include working code examples that readers can compile and flash

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

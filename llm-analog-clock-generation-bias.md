---
title: LLM Analog Clock Generation Bias - The 10:10 Problem
date: 2025-07-03
keywords: llm, ai, bias, chatgpt, image generation, analog clock, representation bias, training data
---

> LLMs struggle to generate analog clocks showing correct time due to training data bias - most watch images show hands at 10:10 for aesthetic/marketing reasons.

## Table of Contents
- [Problem](#problem)
- [Solution](#solution)
- [Mitigation](#mitigation)
- [References](#references)

## Problem

When asked to generate images of analog clocks showing specific times, Large Language Models (LLMs) like ChatGPT consistently fail to position the clock hands correctly. Investigation reveals this is due to a representation bias in their training data:

- Most professional watch/clock photographs show the time as 10:10 (10 minutes past 10)
- This positioning is used in marketing because:
  - It creates a symmetrical, aesthetically pleasing "smile" shape
  - It frames the brand name/logo typically placed at 12 o'clock
  - It doesn't obscure any subdials or date windows
- LLMs have limited exposure to diverse clock hand positions in their training data
- This creates a strong bias toward generating clocks showing approximately 10:10

## Solution

**There is no solution to this problem within current LLM image generation capabilities.**

This is a fundamental limitation arising from training data bias and cannot be resolved through prompting or other techniques.

## Mitigation

- **For ChatGPT users**: Cannot be mitigated - the model will consistently fail at this task
- **For critical applications**: Use programmatic clock generation tools instead of LLM image generation
- **General lesson**: Be aware of representation biases in training data that can lead to systematic failures
- **Verification**: Always verify LLM-generated content, especially for tasks requiring precise visual accuracy

This issue serves as an important reminder about the limitations of LLMs and the need for careful consideration of training data biases when relying on AI-generated content.

## References

- [Screen recording demonstrating the issue in ChatGPT](assets/chatgpt-analog-clock-bias.mp4)
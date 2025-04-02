# Self-ReS: Self-Reflection in Large Vision-Language Models for Long Video Understanding

## Overview

Self-ReS is a novel self-reflective sampling method designed to enhance performance of Large Vision-Language Models (LVLMs) on long video understanding tasks. The approach addresses the limitations of conventional linear frame sampling strategies by dynamically selecting key video fragments based on user prompts.

## Key Features

- **Non-linear spatiotemporal sampling**: Selects key video fragments relevant to the user query, effectively addressing video data non-linearity
- **No additional training required**: Leverages the inherent sparse attention maps of LVLMs to define reflection tokens
- **Performance improvements**: Enhances long-video task accuracy while achieving up to 46% faster inference speed
- **No additional memory requirements**: Operates within the same GPU memory budget as baseline models

## How It Works

Self-ReS introduces independent reflection paths, where each path processes a different segment of the video in parallel. The self-reflective nature of the LLM is expressed in reflection tokens that evaluate the relevancy of visual tokens based on the user query. Once the reflection paths converge, the LLM performs inference using its default context size, focusing on the most salient visual tokens.

## Results

- Improves accuracy on Video-MME and MLVU benchmarks
- Achieves up to 46% faster inference speed over baseline models
- Seamlessly integrates with existing LVLM architectures
- Outperforms models with significantly larger context sizes

## Citation

```bibtex
@inproceedings{pereira2025selfres,
  title={Self-ReS: Self-Reflection in Large Vision-Language Models for Long Video Understanding},
  author={Pereira, João and Lopes, Vasco and Semedo, David and Neves, João},
  booktitle={Proceedings of...},
  year={2025}
}
```

## Coming Soon

Code and model implementations will be made available in the near future. Stay tuned for updates!

# Phase 5 — Stable Diffusion Image Generation

## Objective
Convert each panel's image prompt into a comic illustration.

## Service
```text
services/image_generator.py
```

## Default Model
```text
runwayml/stable-diffusion-v1-5
```

## GPU Detection
The application checks for CUDA:
```python
device = "cuda" if torch.cuda.is_available() else "cpu"
```

## Why It Downloads Several GB
Stable Diffusion is a large AI model. The first run downloads model components and may require several gigabytes of disk space. This is expected.

## Performance
- GPU: generally much faster
- CPU: generation can take several minutes per panel
- More panels: more generation time
- More inference steps: more generation time

## Development Recommendation
Start with:
```text
Panels: 2
Steps: 20
Guidance: 7.5
```

## Prompt Warning
Stable Diffusion's CLIP encoder has a limited token length. Very long prompts may be truncated. Keep image prompts concise.

## Expected Result
An image is produced for each comic panel.

![Status](https://img.shields.io/badge/status-in%20progress-yellow)
![License](https://img.shields.io/badge/license-MIT-blue)

# TrustFrame
Evaluating when AI-generated image detectors should and shouldn't be trusted.

## Motivation
Deepfake detectors perform well on clean data, but real-world images are compressed, resized, and degraded. This project evaluates how common transformations affect model accuracy, confidence calibration, and prediction stability — and defines conditions where human review is warranted.

## Goals
- Measure accuracy degradation under real-world image transformations
- Evaluate confidence calibration (does high confidence = correct prediction?)
- Define reliability thresholds for human-in-the-loop intervention
- Surface failure patterns through visual diagnostics

## Built on top of
[Image-Deepfake-Detectors-Public-Library](https://github.com/truebees-ai/Image-Deepfake-Detectors-Public-Library)

## Structure
```
trustframe/
├── README.md                  ← overview, motivation, demo gif/image
├── LEARNING_LOG.md            ← what I learned along the way
├── TODO.md                    ← living to-do / progress tracker
├── requirements.txt
├── data/
│   └── README.md              ← explains datasets used (no raw images committed)
├── transforms/
│   └── distortions.py         ← blur, compression, brightness, resize
├── eval/
│   ├── pipeline.py            ← core eval loop
│   ├── metrics.py             ← accuracy, confidence, ECE, stability
│   └── thresholds.py          ← "don't trust" logic
├── notebooks/
│   ├── 01_baseline.ipynb
│   ├── 02_distortions.ipynb
│   └── 03_failure_analysis.ipynb
├── results/
│   └── figures/               ← plots, confusion matrices, calibration curves
└── deploy/
    └── api_sketch.py          ← lightweight Flask/FastAPI wrapper (Week 9–10)
```

## Tech Stack
Python, PyTorch, OpenCV, Pandas, Matplotlib

## Dataset
TBD — evaluating FaceForensics++ and CIFAKE

## Timeline
10-week research project targeting a paper submission

## Status
🚧 In progress — Week 1/10

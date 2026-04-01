# TODO

## Week 1–2: Baseline
- [ ] Read and understand truebees repo
- [ ] Get truebees repo running locally
- [ ] Pick 2–3 detectors to evaluate
- [ ] Pick dataset (FaceForensics++ or CIFAKE)
- [ ] Run baseline accuracy/precision/recall on clean data
- [ ] Commit baseline notebook

## Week 3–4: Distortion Pipeline
- [ ] Build distortions.py (blur, JPEG compression, brightness, resize)
- [ ] Run each detector through all distortion types
- [ ] Plot accuracy vs. distortion severity curves

## Week 5–6: Calibration Analysis
- [ ] Pull confidence scores from each model
- [ ] Compute ECE (Expected Calibration Error)
- [ ] Plot reliability diagrams
- [ ] Identify overconfident wrong predictions

## Week 7–8: Thresholds + Failure Patterns
- [ ] Define human-review threshold rules
- [ ] Run ablation to validate thresholds
- [ ] Build visual failure case gallery

## Week 9–10: Paper + Deployment
- [ ] Write paper draft
- [ ] Build FastAPI wrapper
- [ ] Sketch AWS architecture
- [ ] Submit paper
```

Commit it.

---

## Step 3: Create `requirements.txt`
```
torch
torchvision
opencv-python
Pillow
pandas
matplotlib
scikit-learn
numpy
jupyter
fastapi
uvicorn

# PIGEON Reproduction

Research implementation of image geolocation using CLIP-style visual embeddings and S2 Geometry concepts.

## Overview

This repository explores a PIGEON-style approach to predicting geographic locations from images. The goal is to understand how visual embeddings, geographic partitioning, and confidence-based filtering can be combined for image geolocation.

This is a research-backed implementation, not a production geolocation service.

## Problem

Image geolocation is the task of estimating where an image was taken based on visual signals such as architecture, landscape, roads, vegetation, lighting, signs, and other contextual details.

The challenge is that many images contain ambiguous signals. A reliable system needs more than a simple classifier; it needs geographic structure, uncertainty handling, and clear evaluation.

## Approach

- Use a CLIP ViT-B/32-style backbone for image-level visual embeddings.
- Represent geographic regions through S2 Geometry concepts.
- Train/evaluate a prediction flow that maps visual signals toward structured location candidates.
- Apply confidence-based filtering to reduce unreliable predictions.
- Document limitations and failure cases instead of treating every output as equally reliable.

## Tech Stack

- Python
- Jupyter Notebook
- CLIP / ViT-B/32 concepts
- S2 Geometry concepts
- Machine learning experimentation

## Repository Structure

```text
PIGEON_Reproduction/
  notebooks/ or main notebook
  data/                 # not committed if large or restricted
  outputs/              # example predictions or visualizations
  README.md
```

Adjust this structure to match the actual repository files.

## How To Run

```bash
git clone https://github.com/ahsankhizar5/PIGEON_Reproduction.git
cd PIGEON_Reproduction
pip install -r requirements.txt
```

Then open the notebook and run the cells in order.

If there is no `requirements.txt` yet, add one after confirming the exact dependencies.

## Results

Add:

- sample predictions
- evaluation method
- top-k accuracy or distance-based error if available
- examples where confidence filtering helped
- known failure cases

## Limitations

- Results depend heavily on dataset quality and geographic diversity.
- Some images are visually ambiguous and should not receive high-confidence predictions.
- This implementation is for learning/research reproduction, not deployment.

## What I Learned

- How visual embeddings can be used beyond ordinary image classification.
- Why geographic structure matters in location prediction.
- How confidence filtering can make ML outputs more trustworthy.
- How to translate a research idea into an executable ML workflow.

## Contact

For discussion around image geolocation, applied ML, or research implementation:

- LinkedIn: https://www.linkedin.com/in/ahsankhizar/
- GitHub: https://github.com/ahsankhizar5


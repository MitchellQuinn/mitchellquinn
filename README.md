# Mitchell Quinn

**Applied AI / ML Systems Engineer**  
Computer Vision · Evaluation · Runtime Diagnostics · Agentic Workflows · Technical R&D

I build bounded applied-AI systems where model training is only one part of the work.

My current portfolio focuses on the awkward middle where AI systems become testable: synthetic data, preprocessing contracts, evaluation design, runtime integration, trace capture, failure analysis, and explicit claim boundaries.

I am currently looking for applied AI, ML systems, perception, evaluation, diagnostics, research-engineering, and AI-adjacent systems prototyping roles — especially where production engineering discipline and research-style iteration need to coexist.

---

## Start here

### 1. Bounded Monocular Perception

**Fixed-camera vehicle distance/yaw estimation under controlled conditions.**  
Repository: [github.com/MitchellQuinn/bounded-monocular-perception](https://github.com/MitchellQuinn/bounded-monocular-perception)

This is the main portfolio artifact.

It is a bounded computer-vision and applied-ML workspace for testing whether a fixed monocular camera observing a known vehicle in a constrained scene can estimate useful vehicle state, and what breaks when the system moves from synthetic/offline validation into composed live inference.

Evidence of:

- end-to-end applied ML / computer vision system construction
- Unity synthetic-data generation
- OpenCV preprocessing and representation design
- PyTorch training and model evaluation
- ROI localisation and live runtime composition
- camera calibration and apparent-scale alignment
- trace-backed incident analysis
- honest separation of synthetic validation, live-local evidence, and deployment claims

Current selected synthetic tri-stream baseline:

- distance MAE: `0.015856 m`
- distance RMSE: `0.026030 m`
- distance within `0.10 m`: `0.998483`
- yaw mean error: `1.503031°`
- yaw within `5°`: `0.985433`

These are offline synthetic validation metrics, not real-camera deployment accuracy. The live-local work is treated separately through trace-backed runtime evidence and incident analysis.

---

### 2. ClaimLint

**Evidence-bounded agentic repository auditor.**  
Repository: [github.com/MitchellQuinn/claimlint](https://github.com/MitchellQuinn/claimlint)

ClaimLint is a small agentic workflow system for auditing technical repository claims against a selected evidence corpus.

It extracts explicit claims, retrieves candidate evidence, assigns evidence-bounded verdicts, records missing evidence and artifact gaps, and emits structured outputs such as claim reports, remediation tasks, evidence packets, run manifests, and JSONL claim records.

Evidence of:

- agentic workflow design
- claim/evidence separation
- repository audit logic
- manifest-driven execution
- structured artifact generation
- CLI/runtime contract design
- bounded use of LLMs rather than oracle-style prompting

The core question is not “is this project good?” but:

> What can the selected evidence actually support?

---

### 3. Industrial Sound Anomaly Detection

**Machine pump abnormality detection using compact spectral representations.**  
Repository: [github.com/MitchellQuinn/industrial-sound-anomaly-detection](https://github.com/MitchellQuinn/industrial-sound-anomaly-detection)

This project explores industrial sound anomaly detection using custom heightmap-style spectral representations, activity masks, and compact 2D CNN classification.

Evidence of:

- applied ML in a second modality
- audio/signal preprocessing
- STFT-based feature extraction
- custom spectral representation design
- activity-mask channels
- clip-level aggregation
- ROC AUC evaluation
- reporting of generalisation gaps rather than hiding them

Reported balanced validation result:

- clip validation accuracy: `94.79%`
- clip ROC AUC: `0.9926`

A stricter unseen-unit holdout exposed a cross-unit generalisation gap, which is part of the point: the project is treated as an applied ML investigation, not as a polished production detector.

---

### 4. Zero–Infinity Algebra

**Numerical representation research for preserving distinguishability across collapse events.**  
DOI: [10.5281/zenodo.18280702](https://doi.org/10.5281/zenodo.18280702)  
Repository: [github.com/Zero-Infinity-Algebra/ZIA](https://github.com/Zero-Infinity-Algebra/ZIA)

Zero–Infinity Algebra is an independent numerical-representation research project.

It proposes a two-channel scalar formalism, `∞a ⊕ r`, for making information loss explicit in numerical pipelines affected by clipping, saturation, positivity floors, underflow, and singular-entry events.

Evidence of:

- original formal technical reasoning
- mathematical writeup and implementation
- explicit separation of algebraic facts from policy choices
- sustained independent R&D
- technical boundary-setting
- willingness to conclude when a line of work lacks sufficient practical leverage

The project is not my main employment-facing artifact, but it is useful evidence of depth, persistence, and formalisation ability.

---

## What this portfolio is evidence for

- Applied AI / ML systems engineering in bounded domains
- Computer vision and perception prototyping
- Evaluation design and benchmark construction
- Runtime diagnostics and trace capture
- Failure analysis and incident-style investigation
- Synthetic-data generation and synthetic-to-runtime analysis
- Preprocessing/model contract discipline
- Agentic workflow systems
- Technical R&D with explicit non-claims
- Production engineering habits applied to research-style work

---

## What I am looking for

I am especially interested in roles involving:

- applied AI engineering
- ML systems engineering
- computer vision / perception engineering
- AI evaluation and benchmarking
- runtime diagnostics
- technical investigation
- research engineering
- agentic workflow tooling
- validation, verification, and failure analysis for AI-adjacent systems

I am not presenting this portfolio as evidence of broad open-world computer vision, foundation-model research, or mature production deployment in every AI stack. The strongest evidence here is bounded end-to-end ownership, system evaluation, runtime behaviour, and making technical claims inspectable.

---

## Technical areas

### Machine Learning and Data

PyTorch · NumPy · pandas · CNNs · multitask regression · circular regression · keypoint/visibility experiments · evaluation design · reproducibility · deterministic seeding · dataset split design · unseen-unit holdout · model cards · run manifests

### Computer Vision and Perception

OpenCV · monocular geometry · apparent-scale cues · ROI extraction · contour processing · silhouette extraction · foreground masks · ChArUco calibration · camera intrinsics · affine representation transforms · synthetic image generation · runtime diagnostics

### Audio and Signal Processing

STFT feature extraction · custom spectral representations · activity masks · anomaly detection · clip aggregation · ROC AUC evaluation

### Simulation and Runtime Systems

Unity · C# runtime scripting · render textures · procedural generation · PySide6 · Linux · CUDA · tmux · structured artifacts · trace bundles · compatibility checks

### Software Engineering

Python · C# · SQL · JavaScript · CLI tooling · workflow/runtime contracts · structured manifests · testable boundaries · earlier-career ASP.NET / MVC · Windows services · SQL Server · Selenium · production systems

---

## Background

I have 15+ years of software-engineering experience across production systems, services, data workflows, client-facing platforms, support/operations thinking, and technical problem solving.

After a health-related career break, I returned to technical work through self-directed applied ML, computer vision, audio, agentic workflow, and numerical-representation projects. The recent work is deliberately built as an evidence stack: bounded systems, explicit claims, inspectable artifacts, and written technical reasoning.

---

## Current focus

I am currently focused on making this portfolio legible to teams working in applied AI, industrial ML, perception systems, technical diagnostics, and research-engineering contexts.

The centre of gravity is:

> Build the system.  
> Bound the claim.  
> Measure the degradation.  
> Make the failure inspectable.  
> Improve from evidence.

---

## Contact

- Email: [mitchell.quinn@starcroft.net](mailto:mitchell.quinn@starcroft.net)
- GitHub: [github.com/MitchellQuinn](https://github.com/MitchellQuinn)
- CV: available on request

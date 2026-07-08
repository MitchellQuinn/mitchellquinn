# Mitchell Quinn

Software Engineer · Backend & Test Systems · AI/Agentic Developer Tools · Applied ML Systems

Production Software · Automated Validation · Developer Tooling · Runtime Diagnostics · Evidence-Bounded Systems · Agent Continuity · Computer Vision

I am a software engineer with extensive production-systems experience.

My recent work focuses on agentic developer tools, applied ML systems, computer vision, audio ML, and technical R&D, but the through-line is software engineering: building systems with explicit contracts, reliable workflows, testable boundaries, inspectable outputs, recoverable state, and clear failure modes.

I am looking for software engineering roles across backend systems, software test engineering, validation tooling, developer tools, AI engineering, ML systems, runtime diagnostics, and research-engineering-adjacent work.

---

## Software engineering through-line

Across both my earlier production work and my recent independent projects, the recurring pattern is:

> Build the system. Define the contract. Automate the checks. Preserve the evidence. Inspect the failure. Improve the next run.

That shows up in:

* backend and service-oriented engineering
* testable workflow and runtime boundaries
* CLI tools and developer-facing automation
* schema-controlled outputs and validation gates
* reproducible run artefacts and manifests
* durable execution records for long-running agent work
* diagnostic traces and incident-style failure analysis
* applied ML systems where evaluation and runtime behaviour matter as much as model output

The current portfolio is AI-adjacent in several places, but it is not only an AI portfolio. It is evidence of software engineering applied to difficult, ambiguous, failure-prone systems.

---

## Start here

### 1. WorkOverCV

**Evidence-bounded repository work profile generator.**
Repository: [github.com/MitchellQuinn/workovercv](https://github.com/MitchellQuinn/workovercv)

WorkOverCV is a repository analysis workflow that turns public technical repository artefacts into cautious, evidence-bounded work-behaviour review notes.

It is designed for human technical reviewers, hiring teams, founders, engineering managers, and technical recruiters who want to inspect observable repository work without turning GitHub into a score, proxy credential, or automated hiring decision.

WorkOverCV produces reviewable outputs including:

* work-behaviour signals
* evidence gaps
* role-family discussion routes
* follow-up questions
* cautious screening briefs
* structured reports
* validation-controlled artefacts

It does not make hiring decisions, certify competence, infer protected or private traits, or treat popularity metrics as competence metrics.

Evidence of:

* developer-tool design
* agentic workflow architecture
* deterministic local repository scanning
* schema-controlled artefact generation
* fail-closed validation
* safety boundaries for hiring-adjacent tooling
* separation of workflow contracts, runtime documentation, agent adapters, and implementation

Current status: local proof of concept. It is not a hosted service, not a GitHub bot, and not an automated hiring system.

---

### 2. ClaimLint

**Evidence-bounded repository-claim auditor.**
Repository: [github.com/MitchellQuinn/claimlint](https://github.com/MitchellQuinn/claimlint)

ClaimLint is an agentic audit workflow for turning repository claims into structured, checkable evidence objects.

It reads a selected repository corpus, extracts explicit claims, retrieves candidate evidence, records missing evidence or artefact gaps, and renders structured outputs such as claim reports, remediation tasks, evidence packets, run manifests, manifest snapshots, and JSONL records.

The core question is not:

> Is this project good?

The core question is:

> What can the selected repository evidence actually support?

Evidence of:

* workflow and runtime contract design
* claim/evidence separation
* repository audit logic
* manifest-driven execution
* structured report generation
* CLI tooling
* validation-oriented output design
* bounded use of LLMs rather than oracle-style prompting

---

### 3. Agent Working Ledger

**Durable execution ledger for long-running agent tasks.**
Repository: [github.com/MitchellQuinn/agent-working-ledger](https://github.com/MitchellQuinn/agent-working-ledger)

Agent Working Ledger is a small agentic-developer-tooling project for making long-running AI coding-agent work resumable, reviewable, and handoff-safe.

It gives each substantial task a durable, human-readable execution record covering objectives, progress, decisions, validation evidence, blockers, recovery notes, and next actions. It exists because agentic coding work often fails at the boundaries: interrupted sessions, lost context, stale assumptions, validation drift, and handoffs where the next worker cannot tell what actually happened.

The project treats agent work state as something that should be explicit, inspectable, scoped, and safe to abandon or supersede. The Markdown ledger remains the authority; helper tooling and runtime wrappers exist to create, check, summarise, close, supersede, and adapt ledger scopes without redefining the core schema.

It is deliberately not a planner, issue tracker, test runner, source-control replacement, hidden memory system, or claim of universal agent-runtime compatibility.

Evidence of:

* agentic workflow infrastructure design
* task-local execution-state modelling
* human-readable and agent-readable artefact design
* interruption, handoff, and resumption semantics
* validation evidence and blocker tracking
* recovery-state design for context loss and drift
* CLI helper tooling
* runtime-agnostic core specification
* thin adapter/wrapper design for agent environments
* conservative scope boundaries and explicit non-claims

Current status: public alpha source release with documented specification, templates, examples, evals, runtime wrapper material, and helper CLI. It is not claiming production adoption, PyPI publication, or universal agent-runtime compatibility.

---

### 4. Bounded Monocular Perception

**Fixed-camera vehicle distance/yaw estimation under controlled conditions.**
Repository: [github.com/MitchellQuinn/bounded-monocular-perception](https://github.com/MitchellQuinn/bounded-monocular-perception)

This is the main applied-ML / computer-vision portfolio artefact.

It is a bounded computer-vision and applied-machine-learning workspace for testing whether a fixed monocular camera observing a known vehicle in a constrained scene can estimate useful vehicle state, and what breaks when the system moves from synthetic/offline validation into composed live inference.

The project is deliberately narrow:

* one known vehicle family
* one fixed monocular camera geometry
* one constrained movement plane
* controlled full-frame captures
* synthetic training and validation data
* live-local testing under controlled physical conditions

It should be read as a research-engineering artefact, not as a general-purpose vision product.

Evidence of:

* end-to-end applied ML / computer vision system construction
* Unity synthetic-data generation
* OpenCV preprocessing and representation design
* PyTorch training and model evaluation
* ROI localisation and live runtime composition
* PySide6 live-local runtime tooling
* camera calibration and apparent-scale alignment
* trace capture and incident-style failure analysis
* honest separation of synthetic validation, raw-image composed inference, live-local evidence, and deployment claims

Current selected synthetic tri-stream baseline:

* distance MAE: `0.015856 m`
* distance RMSE: `0.026030 m`
* distance within `0.10 m`: `0.998483`
* yaw mean error: `1.503031°`
* yaw within `5°`: `0.985433`

These are offline synthetic validation metrics, not real-camera deployment accuracy.

The live-local work is treated separately through trace-backed runtime evidence and incident analysis. That is the main point of the project: not just training a model, but measuring the degradation introduced by localisation, preprocessing, camera alignment, foreground extraction, representation construction, and live runtime composition.

---

### 5. Industrial Sound Anomaly Detection

**Machine pump abnormality detection using compact spectral representations.**
Repository: [github.com/MitchellQuinn/industrial-sound-anomaly-detection](https://github.com/MitchellQuinn/industrial-sound-anomaly-detection)

This project explores industrial sound anomaly detection using custom heightmap-style spectral representations, activity masks, and compact 2D CNN classification.

It is a second-modality applied-ML artefact: audio/signal rather than image/perception.

Evidence of:

* applied ML outside computer vision
* audio/signal preprocessing
* STFT-based feature extraction
* custom spectral representation design
* activity-mask channels
* compact 2D CNN classification
* clip-level aggregation
* ROC AUC evaluation
* reporting of generalisation gaps rather than hiding them

Reported balanced validation result:

* clip validation accuracy: `94.79%`
* clip ROC AUC: `0.9926`

A stricter unseen-unit holdout exposed a cross-unit generalisation gap. That is part of the value of the project: it is treated as an applied ML investigation, not as a polished production detector.

---

### 6. Zero–Infinity Algebra

**Numerical representation research for preserving distinguishability across collapse events.**
DOI: [10.5281/zenodo.18280702](https://doi.org/10.5281/zenodo.18280702)
Repository: [github.com/Zero-Infinity-Algebra/ZIA](https://github.com/Zero-Infinity-Algebra/ZIA)

Zero–Infinity Algebra is an independent numerical-representation research project.

It proposes a two-channel scalar formalism, `∞a ⊕ r`, for making information loss explicit in numerical pipelines affected by clipping, saturation, positivity floors, underflow, and singular-entry events.

The project includes a formal preprint, C++ reference implementation, Python bindings, tests, and notebooks.

Evidence of:

* original formal technical reasoning
* mathematical writeup and implementation
* explicit separation of algebraic facts from policy choices
* sustained independent R&D
* careful technical boundary-setting
* willingness to conclude when a line of work lacks sufficient practical leverage

ZIA is not my main employment-facing artefact, but it is useful evidence of depth, persistence, and formalisation ability.

---

## How these projects fit together

WorkOverCV, ClaimLint, and Agent Working Ledger are related but distinct:

* **ClaimLint** audits whether repository claims are supported by available evidence.
* **WorkOverCV** uses repository artefacts to produce cautious work-behaviour review notes.
* **Agent Working Ledger** preserves task-local execution state so agentic software work can be interrupted, reviewed, resumed, or handed off without losing decisions, blockers, validation state, or recovery context.

Together, they form the current front door of my agentic systems and developer-tooling work.

Bounded Monocular Perception and Industrial Sound Anomaly Detection show the same engineering pattern applied to ML systems: bounded claims, explicit evaluation, reproducible artefacts, runtime traces, and careful separation between validation evidence and deployment claims.

Zero–Infinity Algebra shows the same pattern applied to formal technical R&D: define the representation, separate facts from policy choices, test the implementation, and be explicit about practical limits.

---

## What this portfolio is evidence for

* Production software engineering carried into current technical work
* Backend-adjacent tooling and workflow systems
* Automated validation and testable runtime boundaries
* Developer tools and CLI workflows
* Agentic workflow systems
* Durable execution-state design for long-running agent tasks
* Agent handoff, resumption, and recovery workflows
* Human-readable / agent-readable protocol design
* Runtime wrapper and adapter design for agent environments
* Evidence-bounded repository review
* Claim/evidence separation and validation-controlled outputs
* Applied AI / ML systems engineering in bounded domains
* Computer vision and perception prototyping
* Evaluation design and benchmark construction
* Runtime diagnostics and trace capture
* Failure analysis and incident-style investigation
* Synthetic-data generation and synthetic-to-runtime analysis
* Preprocessing/model contract discipline
* Technical R&D with explicit non-claims

---

## What this portfolio is not claiming

I am not presenting this work as evidence of:

* broad open-world computer vision
* foundation-model research
* production-ready deployment across every AI stack
* general autonomous systems capability
* automated hiring decision-making
* competence scoring from GitHub popularity
* exhaustive repository auditing
* production adoption of Agent Working Ledger
* universal compatibility across all agent runtimes
* hidden or automatic long-term agent memory
* certification, compliance, or safety assurance

The strongest evidence here is bounded end-to-end ownership, system evaluation, runtime behaviour, explicit claim boundaries, and making technical claims inspectable.

---

## Roles and environments I am looking for

I am especially interested in roles involving:

* software engineering
* backend systems
* software test engineering
* validation tooling
* distributed-system test harnesses
* developer tools
* AI-assisted engineering workflows
* applied AI engineering
* ML systems engineering
* computer vision / perception engineering
* AI evaluation and benchmarking
* runtime diagnostics
* technical investigation
* research engineering
* validation, verification, and failure analysis for AI-adjacent systems

The best fit is likely a team that values:

* explicit contracts
* inspectable outputs
* automated checks
* reliable test environments
* reproducible artefacts
* careful troubleshooting
* engineering judgement under uncertainty
* practical systems work rather than metric theatre

I am particularly focused on Sweden, Germany, and Finland-facing opportunities, while remaining open to high-fit roles elsewhere.

---

## Technical areas

### Software engineering, backend, and validation

Production systems · backend services · service-oriented architecture · SQL-backed systems · asynchronous and long-running processes · testable boundaries · validation workflows · troubleshooting · code review · operational thinking · structured logging and artefacts · reliability-focused engineering

Earlier production background includes ASP.NET / MVC, Windows services, SQL Server, Selenium, client-facing platforms, data workflows, support/operations thinking, and SLA-sensitive software.

### Agentic systems and developer tools

Agentic workflows · repository review systems · evidence-bounded reports · workflow/runtime contracts · task-local execution ledgers · agent handoff and resumption workflows · recovery notes · agent adapters · runtime wrapper material · CLI tooling · schema-controlled artefacts · validation gates · provenance records · fail-closed output checks

### Machine learning and data

PyTorch · NumPy · pandas · CNNs · multitask regression · circular regression · keypoint/visibility experiments · evaluation design · reproducibility · deterministic seeding · dataset split design · unseen-unit holdout · model cards · run manifests

### Computer vision and perception

OpenCV · monocular geometry · apparent-scale cues · ROI extraction · contour processing · silhouette extraction · foreground masks · ChArUco calibration · camera intrinsics · affine representation transforms · synthetic image generation · runtime diagnostics

### Audio and signal processing

STFT feature extraction · custom spectral representations · activity masks · anomaly detection · clip aggregation · ROC AUC evaluation · cross-unit generalisation checks

### Simulation and runtime systems

Unity · C# runtime scripting · render textures · procedural generation · PySide6 · Linux · CUDA · tmux · structured artefacts · trace bundles · model compatibility checks

### Languages and tooling

Python · C# · SQL · JavaScript · CLI tooling · JSON schemas · structured manifests · test-covered pipelines · Git · Linux · Windows · typed backend engineering background with current Python-heavy tooling work

---

## Background

I have 15+ years of software-engineering experience across production systems, services, data workflows, client-facing platforms, support/operations thinking, and technical problem solving.

After a health-related career break, I returned to technical work through self-directed applied ML, computer vision, audio, agentic workflow, developer tooling, and numerical-representation projects.

The recent work is deliberately built as an evidence stack:

* bounded systems
* explicit claims
* inspectable artefacts
* written technical reasoning
* reproducible outputs
* trace-backed failure analysis
* recoverable execution state

The aim is not to pretend the gap did not happen. The aim is to make the technical return legible through current, concrete, inspectable work.

---

## Current focus

I am currently focused on roles where software engineering discipline matters: backend systems, validation tooling, developer tools, applied AI systems, technical diagnostics, evidence-bounded review tooling, agentic workflow infrastructure, and research-engineering contexts.

The centre of gravity is:

> Build useful systems. Keep the claims bounded. Preserve the evidence. Make failure inspectable. Make work state recoverable. Let the work explain the engineer.

---

## Contact

* Email: [mitchell.quinn@starcroft.net](mailto:mitchell.quinn@starcroft.net)
* GitHub: [github.com/MitchellQuinn](https://github.com/MitchellQuinn)
* CV: available on request

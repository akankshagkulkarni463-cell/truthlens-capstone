# TruthLens

An explainable artificial intelligence framework for misleading news detection and news credibility assessment.

TruthLens is a capstone project on an AI-assisted development track. It is intended for readers and evaluators who need more than a fake-or-real label.

In this project, **misleading-news detection** means identifying text that is likely false, distorted, or framed in a way that could mislead. **Credibility assessment** means producing a structured judgment of how trustworthy that item appears. The two are meant to work together: a detection or credibility output should be paired with an explanation of which signals influenced it, so the result can be inspected rather than treated as a black box.

## Problem

Misleading and low-credibility news spreads quickly, and many detection tools only return a score or label. Without a clear rationale, users cannot judge why a claim was flagged, how confident the system is, or what evidence was used. That limits trust and makes the output hard to use in academic or professional settings.

## Objectives

- Detect potentially misleading news content using machine learning methods.
- Assess news credibility in a structured, inspectable way.
- Provide explanations for model outputs (for example, which signals influenced a prediction).
- Keep the system documented, reproducible, and suitable for capstone evaluation.
- Use AI coding assistance without inventing features or hiding what is still unimplemented.

## Technology stack

This repository is in the setup stage. No application source code is present yet.

The project is expected to use:

- **Python** for data processing, modeling, and explainability work
- **Node.js** if a web interface or lightweight API is added later
- Common supporting tools such as virtual environments, package managers, and editor configuration

Specific libraries, models, and frameworks will be recorded here as they are chosen and implemented.

## Planned features

The following are intended capabilities, not current functionality:

- Ingest news text (and, later, related metadata if needed)
- Produce a misleading-news or credibility-related prediction
- Surface explanations that support the prediction
- Present results in a simple, reviewable interface
- Include evaluation notes, limitations, and reproducibility details

## Project status

**Early setup.** The repository currently contains project documentation, license, and ignore rules. Implementation, datasets, models, and user-facing features have not been added yet.

## Project structure

The repository currently contains only the files below. There are no source-code directories or application files yet.

```text
.
├── README.md
├── LICENSE
├── .gitignore
└── CLAUDE.md
```

- **README.md** — Project overview, status, and planned work.
- **LICENSE** — MIT License terms for this repository.
- **.gitignore** — Ignore rules for local environments, secrets, caches, and generated files.
- **CLAUDE.md** — Conventions for AI-assisted development on this project.

## Future scope

Possible later work, depending on research results and time:

- Stronger explainability methods and user-facing explanation quality
- Broader evaluation across news domains and sources
- Improved handling of uncertainty, bias, and failure cases
- Optional extensions such as source-level signals or a more complete web application

Any of these will be marked as implemented only after they exist in the codebase.

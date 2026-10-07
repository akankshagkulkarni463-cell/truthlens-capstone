# CLAUDE.md

Guidance for AI assistants working on **TruthLens**.

## Project context

TruthLens is a capstone project: an explainable AI framework for misleading news detection and news credibility assessment. It is developed on an AI-assisted track. The repository is currently in early setup. Documentation and licensing exist; application source code, models, datasets, and user-facing features do not exist until they are added in later commits.

Do not describe planned work as if it is already implemented. If a feature, API, dataset, model, metric, or UI screen is not in the tree, treat it as absent.

## Role of AI assistance

- Help with focused, reviewable changes that the author can understand and defend.
- Prefer small diffs over large rewrites.
- Ask before expanding scope (new frameworks, new services, new directories, or unrelated refactors).
- Never invent files, results, or capabilities to make the project look complete.
- If the request would require guessing unpublished design decisions, state the assumption or ask.

## Development conventions

- Keep the root tidy. Put code under clear directories when implementation begins (for example `src/`, `tests/`, `docs/`), and update the README only to match reality.
- Prefer explicit names over clever abbreviations.
- Do not commit secrets, API keys, credentials, or local environment files.
- Do not add generated artifacts (virtualenvs, `node_modules`, caches, trained weights, large raw datasets) unless the author explicitly wants a specific small sample tracked.
- Match existing style once source files exist. Until then, use simple, standard layouts for the chosen language.

## Technology expectations

- Python is the expected core language for modeling, evaluation, and explainability.
- Node.js may be used later for a web UI or API. Do not add a frontend or backend stack until it is requested.
- Choose well-known, documented libraries over obscure ones.
- Record real dependencies in the appropriate manifest (`requirements.txt` / `pyproject.toml`, `package.json`) when they are introduced—not before.
- Keep experiments reproducible: note data sources, versions, and evaluation setup in documentation when those pieces exist.

## Coding guidelines

- Write clear, typed or well-annotated code where the language supports it.
- Handle errors visibly; do not swallow failures.
- Separate data loading, model inference, explanation generation, and presentation when those layers exist.
- Add tests alongside behavior that can be tested. Do not add empty test scaffolding without a reason.
- Avoid copy-pasted blocks and unused files.
- Comments should explain intent or constraints, not restate obvious code.

## Documentation expectations

- README.md is the public project summary. Keep status honest.
- Update README, this file, and any technical notes when a real change in architecture or status occurs.
- Do not fill docs with marketing language, unimplemented dashboards, or fake benchmarks.
- When adding a feature, document what it does, how to run it, and what it does not do.
- Cite datasets and third-party models accurately.

## Important rules

1. **No invented implementation.** Do not claim models, APIs, accuracy numbers, or UI flows that are not in the repository.
2. **Stay on task.** Change only what the request needs. Do not “improve” unrelated files.
3. **Keep changes reviewable.** Prefer commits and diffs a supervisor can read in one pass.
4. **Do not hide uncertainty.** If data quality, label definitions, or explanation fidelity are limited, say so in code comments or docs.
5. **Do not commit secrets or large binaries.**
6. **Do not rewrite git history or change license/author unless asked.**
7. **Respect academic integrity.** AI may help write and structure code, but the author must understand and be able to explain every change.
8. **Explanations matter.** When model-facing code exists, preserve a path to inspect why a prediction was produced. Do not optimize that away for a higher score.
9. **Ask rather than guess** on dataset licenses, deployment targets, and grading constraints.

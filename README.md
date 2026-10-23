# LandWatch

Land cover classification and environmental change monitoring from Sentinel-2 satellite images,
built as a production MLOps system. Built step by step following [../PLAN.md](../PLAN.md).

Based on: *Comparative Analysis of Machine Learning Techniques on EuroSAT RGB for
Land Use Land Cover Classification* (ICET 2024).

## Folder layout

| Folder | What goes here |
|---|---|
| `data/raw` | Original scenes and datasets, never edited (DVC-tracked from week 3) |
| `data/interim` | Clean patches and labels |
| `data/processed` | Features and embeddings ready for training |
| `src/landwatch` | Python package: ingest, validate, features, train, predict_scene, serve |
| `tests` | Unit, data and model tests |
| `configs` | `params.yaml`, sensor configs (Sentinel-2, EMIT) |
| `notebooks` | Exploration only — real code moves to `src/` |
| `infra` | Docker, Compose, Kubernetes, Helm, Terraform, Ansible |
| `scripts` | Small shell / helper scripts |
| `docs` | Architecture diagrams and design docs |
| `runbooks` | How to debug and fix things (K8s, GPU, …) |
| `notes` | Daily learning notes (`dayXX.md`) |

## Progress

- [x] Day 1 — repo and layout
- [ ] Day 2 — Linux: `scripts/sysinfo.sh` + systemd timer
- [ ] Day 3 — Python env: uv, ruff, pytest, pre-commit
- [ ] Day 4 — Docker image with GDAL + rasterio, non-root
- [ ] Day 5 — Compose: Postgres + MinIO + geo container
- [ ] Day 6 — Review: list the manual steps in paper 1

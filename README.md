# FitFlow Redesign

Redesign of the FitFlow fitness app (IT3060 Human Computer Interaction, SLIIT - Lab 5).

## Problem
68% of users abandon FitFlow shortly after onboarding. Research (Labs 1-4) shows users need adaptive, explainable AI workout plans, effortless camera-based meal logging, and private low-pressure social features.

## Tech stack
| Layer | Technology |
|---|---|
| Frontend (iOS / Android / Web) | Flutter |
| Core API | NestJS (TypeScript) + WebSocket gateway |
| AI service | Python / FastAPI |
| Database | PostgreSQL (Supabase) |
| Authentication | Supabase Auth |
| Cache / queue | Redis |
| Storage | S3-compatible object storage |

## Repository structure
- `frontend/` - Flutter app
- `backend/` - NestJS core API
- `ai-service/` - FastAPI AI microservice
- `infra/` - Docker and deployment files
- `docs/` - tech stack summary, comparison matrix, architecture diagram, ADRs

## Documentation
- [Tech stack summary](docs/tech-stack-summary.md)
- [Comparison matrix](docs/comparison-matrix.md)
- [Architecture diagram](docs/architecture/architecture-diagram.png)
- [ADR-001: Technology stack](docs/adr/ADR-001-technology-stack.md)

## Contributing
Work on `feature/<name>` branches and open a pull request into `main`. `main` is protected: one approval and a passing CI run are required.

## Author
G.S Oudeen - IT23533714

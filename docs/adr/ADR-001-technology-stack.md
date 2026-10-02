# ADR-001: Technology stack for the FitFlow redesign

- **Status:** Accepted
- **Date:** 2026-10-02

## Context
FitFlow needs a seamless iOS/Android/web experience, an adaptive AI workout engine, camera-based nutrition logging and private social circles. A 68% onboarding drop-off demands rapid iteration. A mid-sized team must handle health data under GDPR/CCPA and keep AI responses within 2 seconds.

## Decision
Flutter for all clients; NestJS core API with WebSocket gateway; FastAPI AI microservice; PostgreSQL and Auth via Supabase; Redis; S3-compatible storage; containers on AWS with GitHub Actions CI/CD.

## Alternatives considered
- React Native + MongoDB + Auth0
- Flutter + Firebase
- Native Swift/Kotlin + Go + DynamoDB + Cognito

## Consequences
- Positive: single UI codebase, Python-native AI, strong privacy via RLS, predictable cost.
- Negative: Dart learning curve, two backend languages, Supabase vendor dependency, Flutter Web SEO limits.

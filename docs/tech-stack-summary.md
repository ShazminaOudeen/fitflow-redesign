# Tech Stack Summary

| Layer | Choice | Why |
|---|---|---|
| Frontend | Flutter | One codebase for iOS, Android and web; smooth camera/animation performance; fast iteration |
| Core API | NestJS | Fast development, modular structure, built-in WebSocket gateways |
| AI service | FastAPI | Native Python ML ecosystem for workout engine and food recognition |
| Database | PostgreSQL (Supabase) | Relational fit, Row Level Security, pgvector, portable |
| Auth | Supabase Auth | JWT, MFA, OAuth, tight RLS integration (fallback: AWS Cognito) |
| Cache / queue | Redis | Plan caching, pub/sub for circles, job queue |
| Storage | S3-compatible | Encrypted meal photos |

Note: verify current vendor pricing and compliance (HIPAA BAA / GDPR DPA) before final adoption.

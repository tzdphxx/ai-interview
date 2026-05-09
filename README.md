# InterviewPilot

InterviewPilot is a personal AI interview practice project built with Spring Boot 4, React 18, PostgreSQL/pgvector, Redis, and S3-compatible storage.

## Features

- Resume upload and AI analysis
- Text mock interviews with answer evaluation
- Voice mock interviews with ASR/TTS support
- Knowledge base upload and RAG question answering
- Interview schedule management
- Runtime LLM provider configuration

## Tech Stack

- Backend: Java 21, Spring Boot 4, Spring AI, Gradle
- Frontend: React 18, TypeScript, Vite
- Data: PostgreSQL with pgvector, Redis
- Storage: MinIO or other S3-compatible services

## Quick Start

1. Copy `.env.example` to `.env` and fill in the provider keys you need.
2. Start local dependencies:

```bash
docker compose -f docker-compose.dev.yml up -d
```

3. Start the backend:

```bash
./gradlew :app:bootRun
```

4. Start the frontend:

```bash
cd frontend
pnpm install
pnpm dev
```

Backend API docs are available at `http://localhost:8080/swagger-ui.html`.

## Docker

```bash
docker compose up -d --build
```

## License

This project is distributed under the GNU Affero General Public License v3.0. See `LICENSE` and `NOTICE` for details.

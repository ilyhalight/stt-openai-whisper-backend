## STT OpenAI Whisper Component

Uses OpenAI Whisper to perform audio transcription using their local models

## How to Run?

### With Docker?

1. Install Docker
2. Build image:

for subscribers

```bash
docker build -t subcriber-custom --build-arg SERVICE=sub:custom .
```

for server

```bash
docker build -t example-backend --build-arg SERVICE=start:cold .
```

3. Run

```bash
docker run --network host subcriber-custom
```

### Without Docker

1. Install Bun
2. Run

for subscribers

```bash
bun sub:custom
```

for server

```bash
bun start:cold
```

## Requirements

- Bun
- NATS
- PostgreSQL
- Redis

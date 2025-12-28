# API Documentation

## Supported APIs

### 1. icanhazdadjoke

**Endpoint:** `https://icanhazdadjoke.com/`

**Method:** GET

**Headers:**
```json
{
  "Accept": "application/json",
  "User-Agent": "Random-Joke-Generator (example)"
}
```

**Response:**
```json
{
  "id": "R7UfaahVfFd",
  "joke": "Why did the coffee file a police report? It got mugged.",
  "status": 200
}
```

---

### 2. Official Joke API

**Endpoint:** `https://official-joke-api.appspot.com/random_joke`

**Method:** GET

**Response:**
```json
{
  "id": 123,
  "type": "general",
  "setup": "What do you call a fake noodle?",
  "punchline": "An impasta!"
}
```

## Rate Limiting

Both APIs are free and don't require authentication. Please be respectful:
- Don't make excessive requests
- Implement caching where possible
- Follow each API's terms of service
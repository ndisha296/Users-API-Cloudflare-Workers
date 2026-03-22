# Users-API-Cloudflare-Workers

# Users API — Cloudflare Workers

A simple REST API built with Cloudflare Workers that performs CRUD operations on users.

## Live Demo
  https://users-api.naikdisha111.workers.dev

## Tech Stack
- Cloudflare Workers
- Wrangler CLI
- JavaScript

## Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/users` | Get all users |
| GET | `/users/:id` | Get a single user by ID |
| POST | `/users` | Create a new user |
| PUT | `/users/:id` | Update a user |
| DELETE | `/users/:id` | Delete a user |

## Example Request

### Create a user (POST)
```json
{
  "name": "Charlie",
  "email": "charlie@example.com"
}
```

### Response
```json
{
  "id": 3,
  "name": "Charlie",
  "email": "charlie@example.com"
}
```

## Getting Started

### Prerequisites
- Node.js
- Cloudflare account

### Installation

1. Clone the repo
```bash
git clone https://github.com/yourname/users-api.git
cd users-api
```

2. Install dependencies
```bash
npm install
```

3. Run locally
```bash
npm run dev
```

4. Deploy to Cloudflare
```bash
npx wrangler deploy
```

## Note
This API uses in-memory storage, meaning data resets on every worker restart.
For persistent storage, integrate with Cloudflare D1.

## Author
Disha

# Financial Track Server

A RESTful API backend for tracking personal financial data, built with Node.js, Express, TypeScript, and MongoDB.

## Tech Stack

- **Runtime:** Node.js
- **Framework:** Express.js
- **Language:** TypeScript
- **Database:** MongoDB (via Mongoose)
- **Tools:** dotenv, CORS, Nodemon

## Project Structure

```
financial-track-server/
├── src/
│   ├── index.ts          # Entry point, server setup
│   ├── routes/           # API route definitions
│   ├── controllers/      # Request handlers
│   └── models/           # Mongoose schemas
├── package.json
└── tsconfig.json
```

## Getting Started

### Prerequisites

- Node.js v18+
- MongoDB (local or Atlas)

### Installation

```bash
git clone https://github.com/meniem13/financial-track-server.git
cd financial-track-server
npm install
```

### Environment Variables

Create a `.env` file in the root directory:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
```

### Running the Server

```bash
# Development
npm run dev

# Production build
npm run build
npm start
```

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/transactions` | Get all transactions |
| POST | `/api/transactions` | Create a new transaction |
| PUT | `/api/transactions/:id` | Update a transaction |
| DELETE | `/api/transactions/:id` | Delete a transaction |

## License

MIT

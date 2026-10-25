# Wanderlust Server

A REST API server built with Express and MongoDB for managing travel destinations.

## Features

- List all destinations
- Get a single destination by id
- Add a new destination

## Setup

1. Install dependencies:

   ```bash
   npm install
   ```

2. Create a `.env` file in the project root:

   ```env
   MONGODB_URL=your-mongodb-connection-string
   ```

3. Start the server:

   ```bash
   node index.js
   ```

The server runs at `http://localhost:8000`.

## API

| Method | Endpoint                 | Description                     |
| ------ | ------------------------ | ------------------------------- |
| GET    | `/`                      | Health check                    |
| GET    | `/destinations`          | Get all destinations            |
| GET    | `/destination/:id`       | Get a destination by id         |
| POST   | `/add-destination`       | Add a destination (JSON body)   |

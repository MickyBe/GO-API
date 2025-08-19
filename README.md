# Go API Example

This project is a simple Go API server demonstrating authentication, middleware, and mock database usage.

## Features

-   REST API with [chi](https://github.com/go-chi/chi)
-   Middleware for authorization
-   Mock database for user login and coin balances
-   Structured logging with [logrus](https://github.com/sirupsen/logrus)

## Project Structure

-   `api/`: API types and error helpers
-   `cmd/api/`: Main entrypoint for the server
-   `internal/handlers/`: HTTP handlers
-   `internal/middleware/`: Middleware (e.g., authorization)
-   `internal/tools/`: Database interface and mock implementation

## Running

```sh
go run ./cmd/api
```

Server runs at `localhost:3000`.

## Example Request

```sh
curl -H "Authorization: 123ABC" "http://localhost:3000/account/coins?username=alex"
```

## License

MIT

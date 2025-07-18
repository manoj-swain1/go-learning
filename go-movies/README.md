# Go Movies REST API

A simple RESTful API for managing movies, built with Go and [Gorilla Mux](https://github.com/gorilla/mux).

## Features

- List all movies (`GET /movies`)
- Get a single movie by ID (`GET /movies/{id}`)
- Create a new movie (`POST /movies`)
- Update an existing movie (`PUT /movies/{id}`)
- Delete a movie (`DELETE /movies/{id}`)

## Movie Model

```json
{
  "id": "string",
  "title": "string",
  "isbn": "string",
  "director": {
    "firstname": "string",
    "lastname": "string"
  }
}
```

## Getting Started

### Prerequisites

- [Go](https://golang.org/dl/) 1.24 or higher
- [Gorilla Mux](https://github.com/gorilla/mux)

Install dependencies:

```sh
go get -u github.com/gorilla/mux
```

### Running the Server

```sh
go run main.go
```

The server will start on [http://localhost:8000](http://localhost:8000).

## API Endpoints

### Get all movies

```
GET /movies
```

### Get a movie by ID

```
GET /movies/{id}
```

### Create a new movie

```
POST /movies
Content-Type: application/json

{
  "title": "Movie Title",
  "isbn": "123456",
  "director": {
    "firstname": "John",
    "lastname": "Doe"
  }
}
```

### Update a movie

```
PUT /movies/{id}
Content-Type: application/json

{
  "title": "Updated Title",
  "isbn": "654321",
  "director": {
    "firstname": "Jane",
    "lastname": "Smith"
  }
}
```

### Delete a movie

```
DELETE /movies/{id}
```

##
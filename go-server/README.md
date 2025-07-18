# Go Server Example

This is a basic Go web server that serves static files and handles simple form submissions.

## Project Structure

```
go-server/
  main.go
  static/
    form.html
    index.html
```

- `main.go`: Main server code.
- `static/index.html`: Static homepage.
- `static/form.html`: HTML form for submitting name and address.

## Running the Server

1. Make sure you have [Go installed](https://golang.org/dl/).
2. Navigate to the `go-server` directory.
3. Run the server:

   ```sh
   go run main.go
   ```

4. Open your browser and visit:
   - [http://localhost:8080/](http://localhost:8080/) for the static homepage.
   - [http://localhost:8080/form.html](http://localhost:8080/form.html) for the form.

## Endpoints

- `/`  
  Serves static files from the `static` directory.

- `/form`  
  Handles POST requests from the form and displays submitted data.

- `/hello`  
  Responds with "Hello" for GET requests.

## Example Form Submission

Submit your name and address at [http://localhost:8080/form.html](http://localhost:8080/form.html). The server will respond with the submitted values.
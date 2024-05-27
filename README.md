# Movies CRUD

This is a simple Go project that implements a CRUD (Create, Read, Update, Delete) API for managing movies.

## Installation

1. Clone the repository:

	```shell
	git clone https://github.com/Diyarbekoralbaev/go-movies-crud.git
	```

2. Change into the project directory:

	```shell
	cd movies-crud
	```

3. Install the dependencies:

	```shell
	go mod download
	```

## Usage

1. Start the server:

	```shell
	go run main.go
	```

	The server will start running on port 8080.

2. Interact with the API using a tool like cURL or Postman.

	- Get all movies:

	  ```shell
	  curl http://localhost:8080/movies
	  ```

	- Get a specific movie:

	  ```shell
	  curl http://localhost:8080/movies/{id}
	  ```

	- Create a new movie:

	  ```shell
	  curl -X POST -H "Content-Type: application/json" -d '{"isbn":"123456","title":"New Movie","director":{"firstname":"John","lastname":"Doe"}}' http://localhost:8080/movies
	  ```

	- Update a movie:

	  ```shell
	  curl -X PUT -H "Content-Type: application/json" -d '{"isbn":"123456","title":"Updated Movie","director":{"firstname":"John","lastname":"Doe"}}' http://localhost:8080/movies/{id}
	  ```

	- Delete a movie:

	  ```shell
	  curl -X DELETE http://localhost:8080/movies/{id}
	  ```

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

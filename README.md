# Rails Devise Passwordless Authentication

https://github.com/abevoelker/devise-passwordless

This application demonstrates how to use Rails with Devise and the `devise-passwordless` gem to implement passwordless authentication. When a user signs in, the app sends a sign-in request to the user's email.

## Getting Started

### Prerequisites

- Ruby (version specified in `.ruby-version`)
- Node.js (version specified in `Dockerfile`)
- PostgreSQL
- Bundler
- bun

### Installation

1. Clone the repository:

    ```sh
    git clone <repository-url>
    cd <repository-directory>
    ```

2. Install Ruby dependencies:

    ```sh
    bundle install
    ```

3. Install JavaScript dependencies:

    ```sh
    bun install
    ```

4. Set up the database:

    ```sh
    rails db:create
    rails db:migrate
    ```

5. Set up environment variables:

    Create a `.env` file in the root directory and add the necessary environment variables.

### Running the Application

1. Start the Rails server:

    ```sh
    rails server
    ```

2. Open your browser and navigate to `http://localhost:3000`.

### Running Tests

To run the test suite, use the following command:

```sh
rails test
```

### CI/CD

This project uses GitHub Actions for continuous integration. The configuration can be found in [`.github/workflows/ci.yml`](.github/workflows/ci.yml).

### Docker

To build and run the application using Docker, use the following commands:

1. Build the Docker image:

    ```sh
    docker build -t myapp .
    ```

2. Run the Docker container:

    ```sh
    docker run -p 3000:3000 myapp
    ```

### Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Open a pull request.

### License

This project is licensed under the MIT License.

### Acknowledgements

- [Devise](https://github.com/heartcombo/devise)
- [devise-passwordless](https://github.com/abevoelker/devise-passwordless)

# Hello, Elegance

A simple, elegant "Hello, World!" Next.js application.

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:9002](http://localhost:9002) with your browser to see the result.

## Docker Deployment

This application is optimized for Docker deployment.

### Using Docker Compose

The easiest way to run this application with Docker is by using Docker Compose.

1.  **Build and run the container:**

    ```bash
    docker-compose up --build -d
    ```
    This command builds the Docker image and starts the container in the background.

2.  **Check the running container and port:**

    To see which port the application is running on, use:
    ```bash
    docker-compose ps
    ```
    Look for the `donegeon_trials` service and check the `PORTS` column. It will show something like `0.0.0.0:49153->3000/tcp`, meaning you can access the app at `http://localhost:49153`.

3.  **View logs:**

    To see the container logs, run:
    ```bash
    docker-compose logs -f
    ```

4.  **Stop the container:**

    ```bash
    docker-compose down
    ```

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

This application is designed to be deployed using Docker.

### Build the Docker Image

From the root of the project, run the following command to build the Docker image:

```bash
docker build -t donegeon_trials .
```

### Run the Docker Container

To run the application inside a Docker container, use the following command.

This command will:
- Name the container `donegeon_trials`.
- Map a random available port on your host machine to port 3000 inside the container.
- Run the container in detached mode (`-d`).

```bash
docker run -d --name donegeon_trials -p 0:3000 donegeon_trials
```

To find out which port the container is mapped to, run:
```bash
docker ps
```
Look for the `donegeon_trials` container and check the `PORTS` column.

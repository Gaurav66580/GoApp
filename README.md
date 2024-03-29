# Go Component for MyApp

This repository contains the Go component for MyApp, a web application. The Go component serves as the backend service.

## Getting Started

### Prerequisites

- Go: Ensure you have Go installed on your system.
- Docker: Ensure you have Docker installed on your system.
- GitHub account: You'll need a GitHub account to set up GitHub Actions.
- Docker Hub account: You'll need a Docker Hub account to push Docker images.

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/GoApp.git
   cd GoApp

2.Set up Docker Hub credentials as GitHub Secrets:

Navigate to your repository on GitHub.
Go to "Settings" -> "Secrets" -> "New repository secret".
Add DOCKER_USERNAME and DOCKER_PASSWORD secrets with your Docker Hub credentials.
Run Tests and Build Locally:

3. Run Tests and Build Locally:
   go test -v ./...
   go build -v .
   
5. docker build -t yourusername/myapp-go:latest .
   
5.docker login -u <your-username> -p <your-password>
  docker push yourusername/myapp-go:latest

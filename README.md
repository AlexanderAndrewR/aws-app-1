# aws-app-1

A containerized Python web app, built with generative AI guidance as a hands-on cloud portfolio project. The application focus is on packaging, deploying, and operating it the way a real production service would be handled.

## Tech stack

- **Python (Flask)** — a minimal web application
- **Docker** — packages the app into a portable container
- **AWS** *(in progress)* — cloud hosting with ECS Fargate
- **Terraform** *(planned)* — infrastructure as code
- **GitHub Actions** *(planned)* — CI/CD pipeline

## To run locally

You'll need [Docker](https://www.docker.com/) installed and running.

Build the container image:

```bash
docker build -t aws-app-1 .
```

Run it:

```bash
docker run -p 8080:8080 aws-app-1
```

Then open http://localhost:8080 in your browser — you should see a greeting served from inside the container.

## Project status

This project is being built in stages:

- [x] Containerized Flask app running locally
- [x] Version-controlled on GitHub
- [ ] Deployed to AWS
- [ ] Infrastructure managed with Terraform
- [ ] Automated CI/CD pipeline
- [ ] Monitoring and secrets management

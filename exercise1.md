# Developing an Application with Python

In this hypothetical development, we're using Python with the framework Django to create a delivery app.

## For Linting, Testing, and Building

- For linting, we're using Flake8 and Black as a code formatter (like ESLint and Prettier for JavaScript-based projects).

- For testing, we're using pytest, a popular framework with simple syntax.

- For building, we're using Poetry.

## Alternatives to Set Up the CI (Besides Jenkins and GitHub Actions)

### Cloud-Based Options:

- GitLab CI/CD: Strong and supports pipelines, Docker, and Kubernetes. This would be a really good option if the team were already using GitLab.

- Bitbucket Pipelines: Easy to set up and recommended for small teams but offers fewer free minutes compared to GitHub and GitLab.

- CircleCI: Easy to configure and good support for Docker.

- Azure Pipelines: Good integration with Microsoft. Supports deployments in Azure/AWS/GCP.

- Travis CI: Easy to set up for open-source projects.

### Self-Hosted Options:

- Drone CI: Light and easy to set up.

- Argo Workflows

- Tekton

- Buildkite

## Best CI Option(s):

To make this decision, the most important and relevant information is how many users we expect to have because if we expect a lot, we need to take care of scalability. In that case, we would prefer an option like Azure. But if we need something light and easy to set up, maybe we can choose Bitbucket or CircleCI. In these cases, the cloud-based options seem like the best.

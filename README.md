# CI/CD Demo Project
This is a sample Node.js project with a Continuous Integration (CI) and Continuous Deployment (CD) pipeline using GitHub Actions. The pipeline automatically runs tests on each push and deploys successful builds to GitHub Pages.

## Project Overview
This repository demonstrates a simple setup of CI/CD with a Node.js application. The CI pipeline ensures that all tests pass before deploying the latest version of the app.

## Features
- Automated Testing: Ensures all tests pass before deployment.
- Continuous Deployment: Deploys the app automatically when changes are pushed to the main branch.
- GitHub Pages Hosting: Builds are deployed to GitHub Pages.

## Getting Started
### Prerequisites
- Node.js and yarn installed
- GitHub account with a repository for the project.

### Installation
Clone the repository and install dependencies:

```

git clone https://github.com/aixdevops/ci-cd-demo.git
cd ci-cd-demo
yarn
```

### Running Tests Locally

To run tests locally:

```
yarn test
```

### Directory Structure

tests/: Contains test files.

.github/workflows/: Contains GitHub Actions workflows for CI/CD.

### CI/CD Pipeline

The GitHub Actions workflow is located in .github/workflows/ci.yml. This workflow:

Runs tests on each push to main.

Deploys to GitHub Pages if tests pass.

## Deployment

The application is automatically deployed to GitHub Pages. You can view the live application at:

https://aixdevops.github.io/ci-cd-demo

## Contributing

Feel free to fork this repository and submit pull requests.

## License

This project is licensed under the MIT License. See the LICENSE.md file for details.
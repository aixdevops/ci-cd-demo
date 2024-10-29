# CI/CD Demo Project
This is a sample Node.js project with a Continuous Integration (CI) and Continuous Deployment (CD) pipeline using GitHub Actions. The pipeline automatically runs tests on each push and deploys successful builds to GitHub Pages.

## Project Overview
This repository demonstrates a simple setup of CI/CD with a Node.js application. The CI pipeline ensures that all tests pass before deploying the latest version of the app.

## Features
- Automated Testing: Ensures all tests pass before deployment.
- Continuous Deployment: Deploys the app automatically when changes are pushed to the main branch.
- GitHub Pages Hosting: Builds are deployed to GitHub Pages.

## Getting Started
### CI/CD Pipeline for Github Pages

You can easily deploy this app to GitHub Pages by following the instructions below. You have two options: **forking this repository** or **cloning and pushing to a new GitHub repository**.

#### Option 1: Fork this Repository

1. **Fork the Repository**:
   - Click the **Fork** button in the upper-right corner of this repository's page on GitHub.

2. **Enable GitHub Actions Permissions**:
   - Go to **Settings > Actions > General** in your forked repository.
   - Under **Workflow permissions**, select **Read and write permissions** and click **Save**.

3. **Enable GitHub Pages**:
   - Go to **Settings > Pages** in your forked repository.
   - Under **Source**, choose **GitHub Actions** as the deployment source.

4. **Trigger Deployment**:
   - After forking and adjusting the settings, the GitHub Actions workflow should run automatically on the `main` branch.
   - Alternatively, you can go to the **Actions** tab and manually trigger the workflow by selecting the **Deploy static content to Pages** workflow and clicking **Run workflow**.

5. **Access the Deployed Site**:
   - Once the workflow completes, your site will be available at `https://<your-username>.github.io/ci-cd-demo`.

#### Option 2: Clone and Push to a New Repository

If you prefer, you can create a new GitHub repository and deploy it manually:

1. **Clone This Repository Locally**:
   ```bash
   git clone https://github.com/aixdevops/ci-cd-demo.git
   ```

2. **Create a New Github Repository**

3. **Set the new repository as the Remote and push:**
  ```bash
  cd your-repo-name
  git remote set-url origin https://github.com/<your-username>/<new-repo-name>.git
  git push -u origin main
  ```
4. **Configure Github Actions and Github Pages:**
- Follow steps 2-5 in Option 1 to enable Actions permissions and set up GitHub Pages for the new repository.

## Installing and Running Tests Locally
**Prerequisites**

Make sure you have the following installed:

- Node.js (version 18 or higher)

**Clone the repository**

```
git clone https://github.com/aixdevops/ci-cd-demo.git
cd ci-cd-demo
```

**Enable Corepack**
```
corepack enable
```

**Install the dependencies**
```
yarn
```

**Run the tests**
```
yarn test
```


### CI/CD Pipeline

The GitHub Actions workflow is located in .github/workflows/ci.yml. This workflow:

- Runs tests on each push to main.

- Deploys to GitHub Pages if tests pass.

## Live Demo

You can view the live demo at:

https://aixdevops.github.io/ci-cd-demo

## Contributing

Feel free to fork this repository and submit pull requests.

## License

This project is licensed under the MIT License. See the LICENSE.md file for details.
# Flask CI/CD Demo

This repository contains a simple Flask app with a GitHub Actions CI/CD pipeline.

## Workflow Details

- Runs tests on every push to `main` and `staging` branches.
- Deploys automatically to the staging environment on pushes to the `staging` branch.
- Deploys automatically to the production environment when a new release tag is created.

## Setting up Secrets

Add the following secrets in your repository settings (if using real deploy scripts):

- `STAGING_DEPLOY_KEY`: Key or token for staging deployment.
- `PRODUCTION_DEPLOY_KEY`: Key or token for production deployment.

## How to use

- Push changes to `staging` branch to trigger tests and staging deploy.
- Push changes to `main` branch to trigger tests.
- Create a release tag to trigger production deployment.

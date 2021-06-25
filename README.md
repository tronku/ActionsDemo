# Actions Demo

This repository was created to give a basic demo of GitHub Actions, a great feature by GitHub to automate all your software workflows, with CI/CD.

You can check the workflow file in `.github/workflows` directory. The project contains a single workflow that posts a comment on the PR created on the `master` branch. Try it yourself by creating a PR!

## Actions used:
- Checkout - https://github.com/marketplace/actions/checkout
- Setup JAVA - https://github.com/marketplace/actions/setup-java-jdk
- Add PR Comment - https://github.com/marketplace/actions/add-pr-comment

## Important points:
- To emit an output value from a step - `echo "::set-output name=key::$value"`
- To get an output value from a step - `${{ steps.step_id.outputs.key }}`
- You can't share values between jobs as each job runs on different runners.

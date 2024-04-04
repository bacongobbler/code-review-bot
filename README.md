# Automated Code Review

This repository demonstrates how you can receive code reviews from OpenAI using GitHub Actions. It includes a github action that runs a code review on every pull request.

The code review is done by performing the following:

1. Fetch the diff of the pull request using [`GrantBirki/git-diff-action`](https://github.com/GrantBirki/git-diff-action)
2. Send the diff to OpenAI for review using the OpenAI API
3. Capture the response and add it as a comment to the pull request

See https://github.com/bacongobbler/code-review-bot/pull/1 for an example.

## Setup

1. Create an OpenAI account and get an API key
2. Add the API key as a secret in your repository with the name `OPENAI_API_KEY`
3. Copy `.github/workflows/code-review.yml` into your repository
4. Create a pull request and see the code review in action
5. ???
6. Profit!

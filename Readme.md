# GitHub Stats Template

This repository serves as a template for creating your own GitHub repositories. It includes a scheduled GitHub Action that generates GitHub stats on a daily basis.

## Getting Started

To use this template, follow these steps:

1. Click on the "Use this template" button to create a new repository based on this template.
2. Clone the newly created repository to your local machine.

## Creating a GitHub Personal Access Token (PAT)

To enable the scheduled GitHub Action, you need to create a GitHub Personal Access Token (PAT). This token should be a classic token, set to never expire, with scopes for read-only repository and profile access. Here's how:

1. Go to GitHub settings.
2. Navigate to "Developer settings" > "Personal access tokens".
3. Click on "Generate new token".
4. Give your token a descriptive name.
5. Set the expiration to "No expiration" or whatever your preference is.
6. For the scopes, select "repo" (for read-only repository access) and "user:email" (for read-only profile access).
7. Click on "Generate token".
8. Copy the generated token. Be sure to save it somewhere safe, as you won't be able to see it again.

## Adding the PAT to the Repository Secrets

After generating your PAT, you need to add it to the repository secrets. Here's how:

1. Go to your repository settings.
2. Navigate to "Secrets".
3. Click on "New repository secret".
4. Name the secret "ACCESS_TOKEN" and paste your PAT in the value field.
5. Click on "Add secret".

## Using the Scheduled Action

With the PAT added to the repository secrets, the scheduled GitHub Action can now run. This action generates GitHub stats daily.

To view the stats, navigate to the "Actions" tab in your repository. Here, you can see the results of each run of the action.

Remember to always keep your PAT safe and never share it with anyone. It's like a password, but for your GitHub account.

Happy coding!

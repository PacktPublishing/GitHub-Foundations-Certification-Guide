# Lab 8.1: Getting Started with GitHub Actions
Let’s do some lab exercises to see how this works.

## Setting Up Your First Workflow
Create a new workflow file in the .github/workflows directory:
1. Navigate to your repository on GitHub.
2. Create a new directory named .github in the root of your repository if it doesn’t already exist.
3. Within the .github directory, create another directory named workflows.
4. Inside the workflows directory, create a new file named first-workflow.yml.
## Define a simple workflow that runs a basic command, such as printing “Hello, World!”:
Apply the following steps:
1. Open the first-workflow.yml file in a text editor.
2. Add the following YAML code to define a simple workflow:
```yml
name: First Workflow

on: [push]

jobs:
  hello_world_job:
    runs-on: ubuntu-latest

    steps:
    - name: Print Hello, World!
      run: echo "Hello, World!"
```
3. Save the file and commit it to your repository.
4. Push the changes to GitHub. This will trigger the workflow to run whenever you push changes to the repository.
## Exploring the GitHub Actions Marketplace
Browse the GitHub Marketplace to find pre-built actions that can be integrated into your workflows:
1. Go to the GitHub Actions Marketplace by navigating to GitHub Marketplace.
2. Use the search bar to find actions that suit your needs. For example, you can search for “linting” or “testing” actions.
3. Explore the available actions by reading their descriptions, usage instructions, and reviews.
## Learn how to incorporate these actions into your workflow files to extend functionality:
1. Select an action from the marketplace that you want to use. For example, choose a popular action like actions/checkout.
2. Read the usage instructions provided on the action’s page. This typically includes how to reference the action in your workflow file.
3. Modify your workflow file to include the action. For example, to use the actions/checkout action, update your first-workflow.yml file as follows:
```yml
name: First Workflow

on: [push]

jobs:
  hello_world_job:
    runs-on: ubuntu-latest

    steps:
    - name: Checkout repository
      uses: actions/checkout@v2

    - name: Print Hello, World!
      run: echo "Hello, World!"
```
4. Save the changes and push them to GitHub. The workflow will now include the pre-built action.
5. We earlier discussed how a step in a job can either run commands or use other actions from GitHub or third parties. These other actions created by third parties are hosted in the GitHub Actions marketplace.


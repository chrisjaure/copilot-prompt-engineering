# Resolving issues

Follow this guide to create a PR that resolves an issue.

<!--
Copilot Instructions:
- Input: GitHub issue number. Prompt if one was not provided.
- Before following this guide, make sure there are no untracked or uncommitted files. If there are, ask the user if they would like to stash them to continue, or if they would like to cancel.
-->

## Step 1: Read the issue description

Read an understand the ticket requirements.

<!--
Copilot Instructions:
- Use the tool get_issue with the provided GitHub issue number.
- Use owner: chrisjaure when looking up issues in this repo.
-->

## Step 2: Plan a solution

Think through possible options and examine the codebase to document a planned approach.

<!--
Copilot Instructions:
- Use the tool sequentialthinking
-->

## Step 3: Execute the plan

Take the plan and act on it:
- Make sure there are no untracked or staged changes.
- Create a new branch from `main` and switch to it.
- Commit your changes to this branch.

<!--
Copilot Instructions:
- Modify the files locally. DO NOT modify files using GitHub tools like `create_or_update_file`
-->

## Step 4: Create a PR

Make sure all your changes are commited to the branch and submit a PR with a brief summary of the changes.

<!--
Copilot Instructions:
- Use the tool create_pull_request
-->
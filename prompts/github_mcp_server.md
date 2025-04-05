# Use GitHub MCP server to create PRs that resolve issues

This describes how to use the [GitHub MCP server](https://github.com/github/github-mcp-server) (configured in [`.vscode/mcp.json`](/.vscode/mcp.json)) to read an issue description and write a PR to resolve it.

Before prompting, make sure you're using [agent mode](https://code.visualstudio.com/docs/copilot/chat/chat-agent-mode).

## Prompt

> Follow [#file:resolving_issues.md](/docs/resolving_issues.md)

## Response

> Got it! I will follow the instructions in the resolving_issues.md file when resolving issues. Let me know if you have a specific GitHub issue number to work on.

## Prompt

> [2](https://github.com/chrisjaure/copilot-prompt-engineering/issues/2)

## Response

> Run `get_issue`

> The issue requires creating a new markdown document titled `debugging_common_errors.md` under the `docs` directory. This document will serve as a guide for troubleshooting and resolving common errors in the project. It includes sections for an introduction, common errors, and best practices, with specific formatting and Copilot instructions.

> I'll now plan a solution for this task.

> Run `sequentialthinking`

> I have planned the structure for the debugging_common_errors.md document. It will include the required sections: Introduction, Common Errors, and Best Practices, with clear markdown formatting and Copilot instructions for future updates.

> Next, I will create a new branch and start working on the document.

> `git status --porcelain`

> There are no untracked or uncommitted files, so I can proceed with creating a new branch and working on the document. I'll create a branch named debugging-common-errors and switch to it.

> `git checkout -b debugging-common-errors main`

> I have successfully created and switched to a new branch named debugging-common-errors. Now, I will create the debugging_common_errors.md document under the docs directory and populate it with the required content.

> debugging_common_errors.md+22-25

> The document debugging_common_errors.md has been successfully created with all the required sections. Next, I will commit the changes to the debugging-common-errors branch.

> `git add docs/debugging_common_errors.md && git commit -m "Add debugging_common_errors.md with common errors and best practices"`

> The new document has been created and committed successfully.

> `git push origin debugging-common-errors`

> The changes in the debugging-common-errors branch have been successfully pushed to the remote repository. I will now proceed to create the pull request.

> Run `create_pull_request`

> The pull request has been successfully created. It includes the new debugging_common_errors.md document with all the required sections. You can view and review the pull request [here](https://github.com/chrisjaure/copilot-prompt-engineering/pull/3). Let me know if there's anything else you'd like to do!
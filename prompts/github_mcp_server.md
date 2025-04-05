# Use GitHub MCP server to create PRs that resolve issues

This describes how to use the [GitHub MCP server](https://github.com/github/github-mcp-server) (configured in [`.vscode/mcp.json`](/.vscode/mcp.json)) to read an issue description and write a PR to resolve it.

Before prompting, make sure you're using [agent mode](https://code.visualstudio.com/docs/copilot/chat/chat-agent-mode).

## Prompt

> Follow [#file:resolving_issues.md](/docs/resolving_issues.md)

## Response

> ...
> Let me know the GitHub issue number to proceed!

## Prompt

> [2](https://github.com/chrisjaure/copilot-prompt-engineering/issues/2)

## Response

> Run `get_issue`

> The issue requires creating a new markdown document titled `debugging_common_errors.md` under the `docs` directory. This document will serve as a guide for troubleshooting and resolving common errors in the project. It includes sections for an introduction, common errors, and best practices, with specific formatting and Copilot instructions.

> I'll now plan a solution for this task.

> Run `sequentialthinking`

> I have planned the structure for the debugging_common_errors.md document. It will include the required sections: Introduction, Common Errors, and Best Practices, with clear markdown formatting and Copilot instructions for future updates.

> Next, I will create a new branch and start working on the document.

> Run `create_branch`

> I have created a new branch named debugging-common-errors-doc to work on the document. Now, I will proceed to create the debugging_common_errors.md file under the docs directory with the required content.

> debugging_common_errors.md+58-1

> The debugging_common_errors.md file has been created with the required sections and content. Next, I will commit the changes and create a pull request for review.

> Run `create_pull_request`

> 
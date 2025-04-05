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

> I have planned the solution to create the required markdown file with the specified sections and structure. I'll now proceed to implement this plan by creating the debugging_common_errors.md file in the docs directory.

> Run `create_or_update_file`

> The debugging_common_errors.md file has been successfully created in the docs directory. It includes the required sections: Introduction, Common Errors, and Best Practices, along with Copilot instructions for future updates.

> I'll now proceed to create a pull request summarizing these changes.

> Run `create_pull_request`

> 
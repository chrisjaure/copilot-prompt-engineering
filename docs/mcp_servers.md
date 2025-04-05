# Configuring MCP Servers

This guide contains detailed instructions on defining inputs, configuring servers, and adding new servers to the `mcp.json` file.

## Overview

The `mcp.json` file is used to define inputs and server configurations for MCP. Each server is defined with a unique key and specifies the command, arguments, and environment variables required to run it.

## Inputs

Inputs are defined under the `inputs` key. For example:

```json
"inputs": [
    {
        "type": "promptString",
        "id": "github_token",
        "description": "GitHub Personal Access Token",
        "password": true
    }
]
```

- `type`: Specifies the type of input (e.g., `promptString`).
- `id`: A unique identifier for the input.
- `description`: A description of the input.
- `password`: If `true`, the input will be hidden (e.g., for sensitive data).

## Servers

Servers are defined under the `servers` key. Each server has the following properties:

- `command`: The command to execute the server.
- `args`: An array of arguments to pass to the command.
- `env`: Environment variables required by the server.

### Example Configuration

Here is an example configuration for three servers:

```json
"servers": {
    "github": {
        "command": "docker",
        "args": [
            "run",
            "-i",
            "--rm",
            "-e",
            "GITHUB_PERSONAL_ACCESS_TOKEN",
            "ghcr.io/github/github-mcp-server"
        ],
        "env": {
            "GITHUB_PERSONAL_ACCESS_TOKEN": "${input:github_token}"
        }
    },
    "sequentialthinking": {
        "command": "docker",
        "args": [
            "run",
            "--rm",
            "-i",
            "mcp/sequentialthinking"
        ]
    },
    "memory": {
        "command": "npx",
        "args": [
            "-y",
            "@modelcontextprotocol/server-memory"
        ]
    }
}
```

### Adding a New Server

To add a new server:

1. Choose a unique key for the server.
2. Specify the `command` to run the server.
3. Define any required `args` and `env` variables.

### Example

To add a server named `exampleServer`:

```json
"exampleServer": {
    "command": "exampleCommand",
    "args": ["arg1", "arg2"],
    "env": {
        "EXAMPLE_ENV_VAR": "value"
    }
}
```

Save the changes to `mcp.json` and restart the MCP environment to apply the configuration.
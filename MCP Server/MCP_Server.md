# MCP Server
Notes about developing and running MCP Servers

# Python SDK

Resource: https://github.com/modelcontextprotocol/python-sdk

## Adding MCP to python project

```
uv init mcp_server1
cd mcp_server1
uv add "mcp[cli]"
```

## Run MCP inspector from uv
From the project path that was initialized with uv
```
uv run mcp dev main.py
```

## Run MCP Inspector manualy

```
npx @modelcontextprotocol/inspector uv run --with mcp[cli] mcp run ~/projects/mcp_server1/main.py
```

## VSCode Integration
To add an MCP Server to VsCode create the file ```.vscode/mcp.json``` and use the template:

```
{
    "servers": {
        "my-mcp-server-c7db4b2e": {
            "type": "stdio",
            "command": "uv",
            "args": [
                "run",
                "--with",
                "mcp[cli]",
                "mcp",
                "run",
                "~/projects/mcp_server1/main.py"
            ]
        }
    }
}
```

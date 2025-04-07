$env:AZURE_DEVOPS_PAT = '<token>'
$env:AZURE_DEVOPS_ORGANIZATION_URL = 'https://microsoft.visualstudio.com'

Development and Debug:

- Run `mcp dev src/mcp_azure_devops/server.py`
- In inspector - command  = python
                arguments = mcp dev src/mcp_azure_devops/server.py

Add to vs code:

- Command - python src....server.py

```json
"az-devops": {
    "type": "stdio",
    "command": "E:\\learn\\mcp\\mcp-azure-devops\\.venv\\Scripts\\python.exe",
    "args": [
        "E:\\learn\\mcp\\mcp-azure-devops\\src\\mcp_azure_devops\\server.py"
    ],
    "env": {
        "AZURE_DEVOPS_PAT" : "<token>",
        "AZURE_DEVOPS_ORGANIZATION_URL" : "https://microsoft.visualstudio.com"
    }
}
```
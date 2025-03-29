**ghidra-re** is a [Nerve](https://github.com/evilsocket/nerve) agent that uses [this Ghidra MCP server](https://github.com/LaurieWired/GhidraMCP) to reverse a target binary with Ghidra.

Make sure the Ghidra MCP server [is installed correctly](https://github.com/LaurieWired/GhidraMCP?tab=readme-ov-file#installation) and copy its `bridge_mcp_ghidra.py` script in `/usr/local/bin` (you can change this path in `agent.yml`).

Install the agent (requires nerve >= 1.4.x):

```bash
# this will download and install (or update) to ~/.nerve/agents
nerve install evilsocket/ghidra-re 
```

By default it will analyze the currently open binary:

```bash
nerve run ghidra-re
```
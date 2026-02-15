# MavenSkills

Tools that make AI coding agents better at building Java projects.

## Maven MCP Server

AI agents (Claude Code, Cursor, Windsurf) run Maven builds through shell commands and parse pages of raw logs — burning tokens on `[INFO] Downloading...` lines. **[Maven MCP](https://github.com/MavenSkills/mcp-server)** is a [Model Context Protocol](https://modelcontextprotocol.io/) server that returns **structured JSON** instead: just the errors, test results, and actionable information.

**50-70x fewer tokens** on passing builds. Up to **600x reduction** on large failures — a real-case Spring Boot project with 205 errored tests went from 5.4 MB to 9 KB.

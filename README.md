# Plugins for Claude

A collection of useful Claude Code plugins by theohbkim, including both custom-built and curated external plugins.

## Quick Start

```bash
/plugin marketplace add theohbkim/plugins-for-claude

/plugin install <plugin-name>
```

## Plugins

| Plugin | Category | Description |
| ------ | -------- | ----------- |
| [document](#document) | Development | Add comprehensive documentation to code |
| [cloudflare-docs](#cloudflare-docs) | Documentation | Cloudflare documentation access and search |
| [cloudflare-observability](#cloudflare-observability) | Monitoring | Cloudflare observability and monitoring tools |
| [cloudflare-workers-bindings](#cloudflare-workers-bindings) | Development | Cloudflare Workers bindings management |
| [cloudflare-workers-builds](#cloudflare-workers-builds) | Deployment | Cloudflare Workers build and deployment tools |
| [context7](#context7) | Development | Up-to-date documentation lookup from source repositories |
| [filesystem](#filesystem) | Development | Filesystem operations and file management |
| [firecrawl](#firecrawl) | Integration | Web scraping and search capabilities |
| [magic](#magic) | Utility | AI-driven UI component creation |
| [memory](#memory) | Utility | Knowledge graph-based persistent memory |
| [sequential-thinking](#sequential-thinking) | Utility | Dynamic and reflective problem-solving |
| [vercel](#vercel) | Deployment | Vercel deployments and projects |

## Plugin Details

### document

Add comprehensive documentation to code (functions, classes).

**Features:**
- Supports Python (Google-style docstrings) and TypeScript/JavaScript (JSDoc)
- Documents functions and classes with descriptions, parameters, return values, and examples
- Follows existing project documentation style when present
- Works with file paths or IDE selection

**Usage:**

```bash
# Document a specific file
/document src/utils/helpers.py

# Or select code in your IDE and run without arguments
/document
```

### cloudflare-docs

Access and search Cloudflare documentation directly from Claude Code.

**Homepage:** [Cloudflare MCP Documentation](https://developers.cloudflare.com/agents/model-context-protocol/)

### cloudflare-observability

Monitor and observe your Cloudflare infrastructure with integrated observability tools.

**Homepage:** [Cloudflare MCP Documentation](https://developers.cloudflare.com/agents/model-context-protocol/)

### cloudflare-workers-bindings

Manage Cloudflare Workers bindings including KV namespaces, Durable Objects, and more.

**Homepage:** [Cloudflare MCP Documentation](https://developers.cloudflare.com/agents/model-context-protocol/)

### cloudflare-workers-builds

Build and deploy Cloudflare Workers with integrated CI/CD tools.

**Homepage:** [Cloudflare MCP Documentation](https://developers.cloudflare.com/agents/model-context-protocol/)

### context7

Pull version-specific documentation and code examples directly from source repositories into your LLM context using Upstash Context7.

**Homepage:** [Context7 Documentation](https://context7.com/docs/clients/claude-code)

### filesystem

Perform filesystem operations including reading, writing, searching, and managing files and directories.

**Homepage:** [MCP Filesystem Server](https://github.com/modelcontextprotocol/servers/tree/main/src/filesystem)

### firecrawl

Web scraping and search capabilities powered by Firecrawl for extracting structured data from websites.

**Homepage:** [Firecrawl MCP Server](https://docs.firecrawl.dev/mcp-server)

### magic

AI-driven tool that helps developers create beautiful, modern UI components instantly through natural language descriptions.

**Homepage:** [Magic MCP](https://github.com/21st-dev/magic-mcp)

### memory

Knowledge graph-based persistent memory system that helps maintain context across conversations.

**Homepage:** [MCP Memory Server](https://github.com/modelcontextprotocol/servers/tree/main/src/memory)

### sequential-thinking

Dynamic and reflective problem-solving with structured thinking processes for complex tasks.

**Homepage:** [MCP Sequential Thinking Server](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking)

### vercel

Manage Vercel deployments, projects, and infrastructure directly from Claude Code.

**Homepage:** [Vercel MCP Documentation](https://vercel.com/docs/mcp/vercel-mcp)

## Project Structure

```
plugins-for-claude/
├── .claude-plugin/
│   └── marketplace.json       # Marketplace configuration
├── plugins/
│   └── document/
│       ├── .claude-plugin/
│       │   └── plugin.json    # Plugin metadata
│       └── commands/
│           └── document.md    # Command definition
├── LICENSE
└── README.md
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

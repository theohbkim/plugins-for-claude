# Plugins for Claude

A collection of useful Claude Code plugins by theohbkim.

## Quick Start

```bash
/plugin marketplace add theohbkim/plugins-for-claude

/plugin install <plugin-name>
```

## Plugins

| Plugin | Description |
|--------|-------------|
| document | Add comprehensive documentation to code |

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

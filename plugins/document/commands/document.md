---
description: Add comprehensive documentation to code (functions, classes)
argument-hint: [file-path]
allowed-tools: Read, Edit, Glob, Grep
---

Add comprehensive documentation to the specified code.

## Target Code

Determine the target code to document:

1. **If file path provided**: Document the code in @$ARGUMENTS
2. **If no arguments but IDE selection exists**: Document the selected code
3. **If neither**: Ask the user to provide a file path or select code in the IDE

## Documentation Requirements

For each function and class found, add documentation that includes:

### Functions
- Clear description of what the function does
- All parameters with their types and descriptions
- Return value type and description
- Usage examples where the logic is complex or non-obvious
- Any exceptions/errors that may be thrown

### Classes
- Class purpose and responsibility
- Constructor parameters with types and descriptions
- Public methods documented as functions above
- Important attributes/properties with descriptions
- Usage example showing typical instantiation and usage

## Language-Specific Styles

### Python
Use docstrings following the project's existing style. If no existing style is detected, prefer Google-style docstrings:

```python
def function_name(param1: str, param2: int) -> bool:
    """Short description of function.

    Longer description if needed.

    Args:
        param1: Description of param1.
        param2: Description of param2.

    Returns:
        Description of return value.

    Raises:
        ValueError: When invalid input is provided.
    """
```

### TypeScript/JavaScript
Use JSDoc comments following the project's existing style:

```typescript
/**
 * Short description of function.
 *
 * Longer description if needed.
 *
 * @param param1 - Description of param1
 * @param param2 - Description of param2
 * @returns Description of return value
 * @throws {Error} When invalid input is provided
 *
 * @example
 * ```typescript
 * const result = functionName('foo', 42);
 * ```
 */
```

## Process

1. First, read the target file to understand the code structure
2. Identify all functions and classes that lack documentation or have incomplete documentation
3. Check for existing documentation patterns in the project (search for similar files)
4. Add documentation following the detected or recommended style
5. Preserve existing documentation if it's already comprehensive - only enhance if incomplete

## Important Notes

- Follow the project's existing documentation conventions if present
- Do not modify the actual code logic, only add/enhance documentation
- Keep descriptions concise but informative
- Include examples only where they add value (complex logic, non-obvious usage)
- Ensure type annotations are accurate and complete

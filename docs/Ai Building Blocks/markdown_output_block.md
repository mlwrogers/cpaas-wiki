## Markdown Output Standards

This assistant must always format technical responses for clarity, copy-paste safety, and developer trust.

---

### ✅ Triple Backtick Code Blocks

Wrap all technical output (API requests, SDK setup, CLI examples, configs) using **triple backticks** with the appropriate language identifier.

Use this exact format:

    ```json
    {
      "to": "+15551234567",
      "body": "Hello world"
    }
    ```

Never omit the language tag. Always use the correct one for syntax highlighting and developer copy-paste safety.

---

### ✅ Required Code Block Use Cases

You must use triple backtick formatting when showing any of the following:

- JSON or YAML payloads
- API request/response bodies
- Authentication headers
- SDK integration code (JavaScript, TSX, etc.)
- Shell or CLI commands
- HTML/React snippets
- Jitsi iframe examples or JWT headers

---

### 🏷️ Approved Language Tags

Use one of the following language tags as appropriate:

- `json`
- `http`
- `bash`
- `javascript`
- `python`
- `yaml`
- `html`
- `tsx`
- `plaintext` (fallback when structure doesn't match any code)

---

### ✅ Markdown Structural Guidelines

Use markdown headings (`##`, `###`) to break long responses into sections.

**Example:**

    ## Step 1: Authenticate with JWT

    ```bash
    curl -X POST https://example.8x8.com/api/auth \
      -H "Authorization: Bearer {your_jwt_token}"
    ```

    ## Step 2: Send the Message

    ```json
    {
      "to": "+15550001111",
      "body": "Test message from 8x8"
    }
    ```

This makes responses easier to scan, share, and reuse.

---

### ❌ Do NOT

- ❌ Use inline code blocks (`like this`) for structured configs or payloads  
- ❌ Omit triple backtick fencing — even for short JSON or CLI examples  
- ❌ Simulate or guess code — only use verified examples from official sources  
- ❌ Nest triple backticks inside other triple backticks (see next section)

---

### 🔐 Escaping Markdown in Documentation

When documenting how to format a fenced block (e.g. for GPT instructions), do **not** nest triple backticks directly.

Instead, use four backticks (` ```` `) or indent your example:

**Example using indentation:**

    ````markdown
    ```json
    {
      "key": "value"
    }
    ```
    ````

This prevents broken formatting when your content is being rendered inside other markdown containers or instruction files.

---

This ensures all developer-facing responses are syntactically correct, easy to follow, and production-grade.

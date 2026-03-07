# AI_devs 4: Builders

## Lesson 01 Setup

This setup is shared by:

- `01_01_interaction`
- `01_01_structured`
- `01_01_grounding`

Configure your API key once in the workspace root and reuse it across all examples.

### API Keys

Create `.env` in the workspace root (you can copy `env.example`).

Edit `.env` and set one key:

```bash
OPENAI_API_KEY=your_api_key_here
# or
OPENROUTER_API_KEY=your_api_key_here
```

Optional: if both keys are set, choose provider explicitly:

```bash
AI_PROVIDER=openai
# or
AI_PROVIDER=openrouter
```

### Run examples

```bash
npm run lesson1:install
```

```bash
npm run lesson1:interaction
```

```bash
npm run lesson1:structured
```

```bash
npm run lesson1:grounding
```

For `01_01_grounding`, anything after the first `--` is passed to `app.js`.
Use a file name to target one note, and `--force` to ignore cache.

```bash
# Process one file from 01_01_grounding/notes/
npm run lesson1:grounding -- my-note.md

# Rebuild outputs even when cache exists
npm run lesson1:grounding -- --force

# Specific file + force rebuild
npm run lesson1:grounding -- my-note.md --force
```

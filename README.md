# HuggingFace Dataset Creator Skill

Create and manage any type of dataset on HuggingFace Hub through Claude Code. Supports chat/conversational, classification, Q&A, completion, tabular data, and custom formats.

## Setup

1. **Install HuggingFace MCP Server** for dataset discovery:
   ```bash
   claude mcp add hf-mcp-server -t http https://huggingface.co/mcp?login
   ```

2. **Set HuggingFace Token** (get from [settings](https://huggingface.co/settings/tokens)):
   ```bash
   export HF_TOKEN="your_token_here"
   ```

3. **Install dependencies**:
   ```bash
   uv add huggingface_hub
   ```

## Usage in Claude Code

### Quick Start
```
Create a sentiment classification dataset at "myusername/sentiment-data"
```

### Available Dataset Types
- **`chat`** - Conversational AI, assistants, tool usage
- **`classification`** - Sentiment, intent, topic classification
- **`qa`** - Question-answering, reading comprehension
- **`completion`** - Text/code completion, creative writing
- **`tabular`** - Structured data for ML
- **`custom`** - Your own schema

### Example Prompts
```
"Create a Q&A dataset about Python programming at claude-ai/python-qa-dataset"

"Set up a chat dataset for training customer service bots at mycompany/support-chat-data"

"Make a text classification dataset for email categorization at team/email-classifier-data"

"Add 50 more examples to myusername/sentiment-data with positive and negative movie reviews"

"Show me the statistics for claude-ai/python-qa-dataset"
```

### Workflow Integration
The skill works with HuggingFace MCP server:
1. **Discover** existing datasets using HF MCP tools
2. **Create** new datasets with this skill
3. **Manage** content and validation with this skill

## Templates & Validation

Each dataset type includes:
- **Automatic validation** for data quality
- **Schema enforcement** for consistency
- **Example data** to get started quickly
- **Custom system prompts** optimized for the data type

## Links
- [HuggingFace Hub](https://huggingface.co/)
- [HuggingFace MCP Server](https://huggingface.co/mcp)
- [Claude Code Skills](https://code.claude.com/docs/en/skills)
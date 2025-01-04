# Agent-Prompts

A collection of carefully crafted prompts to help you get better results when working with various AI language models (LLMs).

## Purpose

This repository contains optimized prompts for different AI models to help you:
- Get more accurate and consistent responses
- Improve code generation quality
- Achieve better formatting and structure in outputs
- Save time by using tested prompt templates

## Important Note About Using These Prompts

Due to the detailed and specific nature of these prompts, you may occasionally experience:
- LLM timeouts or hanging responses
- Incomplete or truncated outputs
- Error messages from the AI service

This is normal behavior when working with complex prompts. If you encounter these issues:
1. Try breaking your request into smaller chunks
2. Submit the same prompt again (responses may vary)
3. Slightly rephrase the prompt while keeping the core instructions
4. Wait a few moments before retrying if the service seems overwhelmed

## Available Prompts

### Documentation
All prompt templates are available in the Docs folder for easy copying and pasting:
- [Python to Node.js Conversion Guide](./Docs/PythonToNodejs.md) - A comprehensive prompt template for converting Python code to Node.js format.
- [Python to Node.js Large Files Guide](./Docs/PythonToNodejsLargeFiles.md) - A specialized template for handling large file conversions incrementally.
- [Python to Node.js V2 Guide](./Docs/PythonToNodejs-V2.md) - The enhanced version combining best practices from all templates.

### NPM Package Usage
This repository is also available as an npm package for programmatic usage in your projects:

```bash
npm install @MotoAcidic/Agent-Prompts
```

The package includes utility functions for working with your preferred LLM:

- [pythonToNodejs.mjs](./Prompts/pythonToNodejs.mjs) - Provides structured prompts and conversion utilities
- [index.mjs](./index.mjs) - Main entry point with the `fetchLLMPrompt` function

Example usage in your project:
```javascript
import { fetchLLMPrompt } from '@MotoAcidic/Agent-Prompts';
import { getInitialConversionPrompt } from '@MotoAcidic/Agent-Prompts/Prompts/pythonToNodejs.mjs';

// Get the structured prompt
const prompt = getInitialConversionPrompt();

// Send to your LLM
const response = await fetchLLMPrompt('your-llm-model', prompt);
```

## Contributing

Feel free to contribute your own tested prompts by submitting a pull request. Please ensure your prompts are well-documented and include examples of expected outputs.

## License

MIT License - Feel free to use these prompts in your projects
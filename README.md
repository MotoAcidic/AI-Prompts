# AI-Prompts

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

### GitHub Copilot
- [Python to Node.js Conversion Guide](./Copilot/PythonToNodejs.md) - A comprehensive prompt designed to work with GitHub Copilot's `/edit` command for converting Python code to Node.js format. Use this prompt by copying it into a Copilot chat session followed by your Python code when requesting edits.
- [Python to Node.js Large Files Guide](./Copilot/PythonToNodejsLargeFiles.md) - A specialized prompt for converting large Python files to Node.js format using an incremental approach. This guide helps break down large files into manageable chunks to avoid LLM timeout issues and provides a structured process for handling complex conversions.

## Contributing

Feel free to contribute your own tested prompts by submitting a pull request. Please ensure your prompts are well-documented and include examples of expected outputs.

## License

MIT License - Feel free to use these prompts in your projects
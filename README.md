# 🎭 StageHand AI Agent

[![GitHub stars](https://img.shields.io/github/stars/AminePro7/StageHand-AI-Agent?style=social)](https://github.com/AminePro7/StageHand-AI-Agent/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/AminePro7/StageHand-AI-Agent?style=social)](https://github.com/AminePro7/StageHand-AI-Agent/network/members)
[![GitHub issues](https://img.shields.io/github/issues/AminePro7/StageHand-AI-Agent?style=social)](https://github.com/AminePro7/StageHand-AI-Agent/issues)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

## 🚀 Overview

StageHand AI Agent is a powerful browser automation tool built on top of [Playwright](https://playwright.dev/) that provides a higher-level API with AI-powered capabilities for web automation. This project leverages the [Stagehand SDK](https://github.com/browserbasehq/stagehand) to create robust, intelligent browser agents.

## ✨ Features

- 🤖 **AI-Powered Automation**: Use `extract`, `observe`, and `act` methods to intelligently interact with web pages
- 🔍 **Smart Selectors**: Automatically find and interact with elements even when selectors change
- 🛡️ **Graceful Fallbacks**: AI fallbacks when traditional automation methods fail
- 📊 **Detailed Logging**: Comprehensive logging for debugging and monitoring
- ☁️ **Browserbase Integration**: Optional cloud execution environment

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/AminePro7/StageHand-AI-Agent.git

# Navigate to the project directory
cd StageHand-AI-Agent/Agent

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your API keys
```

## 🏃‍♂️ Usage

```bash
# Start the agent
npm start
```

## 📋 Configuration

The agent can be configured in `stagehand.config.ts`:

- Change execution environment (LOCAL/BROWSERBASE)
- Configure AI model settings
- Set timeouts and debugging options
- Customize logging behavior

### Using Anthropic Claude 3.5 Sonnet

1. Add your API key to `.env`
2. Change `modelName: "gpt-4o"` to `modelName: "claude-3-5-sonnet-latest"` in `stagehand.config.ts`
3. Change `modelClientOptions: { apiKey: process.env.OPENAI_API_KEY }` to `modelClientOptions: { apiKey: process.env.ANTHROPIC_API_KEY }` in `stagehand.config.ts`

## 📚 Example

The default example demonstrates:

1. Navigating to the Browserbase documentation
2. Extracting information about the quickstart guide
3. Observing links in the 'Guides' section
4. Clicking the first link using Playwright (with AI fallback)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👤 Author

**AminePro7**

- GitHub: [@AminePro7](https://github.com/AminePro7)

## 🙏 Acknowledgments

- [Browserbase](https://browserbase.com) for the Stagehand SDK
- [Playwright](https://playwright.dev/) for the browser automation foundation

---

<p align="center">Made with ❤️ by <a href="https://github.com/AminePro7">AminePro7</a></p> 
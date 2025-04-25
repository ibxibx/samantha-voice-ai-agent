# 🎙️ Samantha Voice AI Agent

<div align="center">
  <img src="https://raw.githubusercontent.com/ibxibx/samantha-voice-ai-agent/main/workflow-pictures/logo.jpeg" alt="Samantha Logo" width="200"/>
  <h3>Your AI companion just a call away</h3>
  <p>A no-code voice AI assistant that saves your ideas to Google Drive</p>
  
  [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
  [![n8n](https://img.shields.io/badge/Built%20with-n8n-orange)](https://n8n.io/)
  [![OpenAI](https://img.shields.io/badge/Powered%20by-OpenAI-lightgrey)](https://openai.com/)
</div>

## 📋 Overview

Samantha is a voice-activated AI agent built entirely without writing code. She's accessible through a simple phone call and can assist with brainstorming, fact-checking, note-taking, and more. All conversations can be automatically saved to your Google Drive for future reference.

Perfect for when your hands are busy - cooking, driving, exercising - Samantha is always ready to help.

## ✨ Features

- 🗣️ **Natural Voice Interface** - Have conversations with a human-like AI assistant
- 📝 **Google Drive Integration** - Save conversation summaries directly to your cloud
- 🧠 **Powered by GPT-4o** - Benefit from advanced AI capabilities
- 📱 **Phone Accessibility** - Use from any phone without needing an app
- 🔄 **No-Code Implementation** - Built entirely using n8n workflows

## 🛠️ Technical Architecture

Samantha is built on a modern tech stack:

- **n8n** - Workflow automation platform that connects all components
- **Vapi.ai** - Voice AI platform for natural speech interface
- **OpenAI API** - Powers the intelligence with GPT-4o-mini
- **Google Drive API** - Stores conversation summaries in the cloud

### Workflow Architecture

```
┌─────────────┐     ┌───────────┐     ┌─────────────┐     ┌─────────────┐
│   Webhook   │────▶│ AI Agent  │────▶│ Google Docs │────▶│ Update Docs │
│   (Input)   │     │ (Process) │     │  (Create)   │     │  (Output)   │
└─────────────┘     └───────────┘     └─────────────┘     └─────────────┘
```

## 🚀 How It Works

1. **User places a call** to Samantha's phone number
2. **Vapi.ai** handles the voice conversation
3. **Webhook** triggers the n8n workflow when save is requested  
4. **AI Agent** processes and summarizes the conversation
5. **Google Docs nodes** create and update documents with the summary

## 📄 Configuration

The entire implementation is contained in the `Voice-AI-Agent-Samatha-Workflow.json` file in this repository. This workflow can be imported into n8n to recreate the agent.

### Prerequisites:
- n8n account
- OpenAI API key
- Vapi.ai account
- Google account with Drive and Docs enabled

## 🧩 Installation

1. Clone this repository
2. Import the JSON workflow into n8n
3. Configure credentials for:
   - OpenAI API
   - Google Drive/Docs API
4. Set up a voice assistant in Vapi.ai with the webhook URL
5. Test your installation by calling the provided phone number

## 🔮 Future Enhancements

- Calendar integration for scheduling and reminders
- Web search capabilities
- Multi-user support
- Custom voice and personality options
- Integration with other productivity tools

## 👤 About the Developer

Built by Ian Baumeister as a portfolio project demonstrating no-code AI agent development. Special thanks to Aemal Sayer for guidance and mentorship throughout the development process.

## 📜 License

This project is licensed under the MIT License - see the LICENSE file for details.
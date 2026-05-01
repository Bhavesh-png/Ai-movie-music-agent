# AI Movie & Music Agent 🎬🎵

An AI-powered assistant built with **n8n** that provides movie recommendations, music discovery, news headlines, and weather updates through a conversational interface.

## ✨ Features

- **Movie Discovery**: Search for movies, genres, or recommendations using the iTunes database.
- **Music Search**: Find songs, artists, and playlists.
- **Real-time News**: Get the latest global headlines via RSS feeds from BBC, CNN, and more.
- **Weather Forecasts**: Accurate weather data anywhere in the world using Open-Meteo.
- **Intelligent Conversations**: Powered by Google Gemini with memory of past interactions.

## 🚀 Setup Instructions

### Prerequisites
- An instance of [n8n](https://n8n.io/) (Desktop, Cloud, or Self-hosted).
- A [Google Gemini API Key](https://aistudio.google.com/app/apikey).

### Installation
1. Download the `workflow.json` file from this repository.
2. In n8n, click on **Workflows** > **Import from File...** and select `workflow.json`.
3. Configure your credentials:
   - Click on the **Connect Gemini** node.
   - Select or create a new "Google Gemini(PaLM) Api" credential and paste your API key.
4. Click **Execute Workflow** or use the **Chat** interface to start talking to your agent.

## 🌐 Deployment (Render)

This repository is optimized for deployment on **Render** as a Web Service.

1. Create a new **Web Service** on Render and connect this repository.
2. Render will automatically detect the `package.json` and use `npm start` to run the landing page.
3. Once deployed, you will have a professional landing page showcasing your agent!

## 🖥️ Local Development

To run the landing page locally:
```bash
npm install
npm run dev
```
Visit `http://localhost:3000` to see your new landing page.

## 🛠️ Built With
- [n8n](https://n8n.io/) - Workflow automation.
- [Google Gemini](https://deepmind.google/technologies/gemini/) - AI Model.
- [iTunes Search API](https://performance-developer.apple.com/documentation/itunes_store_web_service_toolkit/searching_the_itunes_store) - Movies & Music data.
- [Open-Meteo](https://open-meteo.com/) - Weather data.

---
Built with ❤️ for the n8n community.

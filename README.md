# Multi-Agent Marketing Campaign System

This project demonstrates a **multi-agent AI system** designed to automate marketing campaign creation using Google ADK (Agent Development Kit) and language models like Gemini-2.0. The system is composed of specialized agents working in tandem to handle various tasks, from market research to ad copywriting, visual design, and final campaign orchestration.

## Features

- **Market Research Agent**: Uses Google Search to gather insights about the target market.
- **Messaging Strategist Agent**: Crafts key messaging based on market research.
- **Ad Copywriter Agent**: Generates multiple variations of ad copy based on messaging.
- **Visual Suggester Agent**: Suggests visual concepts to pair with ad copy.
- **Campaign Brief Formatter**: Compiles everything into a final campaign brief in Markdown format.
- **Sequential Orchestrator**: Manages the flow of agents and ensures they work together seamlessly to create the final campaign.

---

## Tech Stack

- **Python**: The primary language for building the agents and orchestration logic.
- **Google ADK**: Used for managing AI agents and orchestrating their workflows.
- **dotenv**: For managing environment variables like API keys.
- **Google Search API**: Used by the Market Research Agent to gather insights.

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/marketing-campaign-agent.git
cd marketing-campaign-agent

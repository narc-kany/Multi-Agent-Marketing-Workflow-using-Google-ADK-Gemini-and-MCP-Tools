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
2. Install Dependencies
Create a virtual environment and install the necessary Python dependencies.

bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # For macOS/Linux
venv\Scripts\activate     # For Windows
pip install -r requirements.txt
3. Setup Environment Variables
Create a .env file in the root directory to store your API keys and model configuration.

plaintext
Copy
Edit
GOOGLE_GENAI_MODEL=gemini-2.0-flash
Make sure to replace gemini-2.0-flash with the correct model name you're using. If you're using any other services (e.g., Google Search API), make sure to add those keys to the .env file as well.

Usage
To start the marketing campaign automation pipeline, simply run the main script:

bash
Copy
Edit
python run_campaign.py
The script will:

Start with the Market Research Agent to gather market insights.

Pass the insights to the Messaging Strategist Agent to craft messaging.

Feed the messaging into the Ad Copywriter Agent for generating ad copy.

Pass the ad copy to the Visual Suggester Agent for visual concepts.

Compile everything into a final campaign brief using the Formatter Agent.

Project Structure
markdown
Copy
Edit
marketing-campaign-agent/
│
├── agents/
│   ├── __init__.py
│   ├── market_research_agent.py
│   ├── messaging_strategist_agent.py
│   ├── ad_copywriter_agent.py
│   ├── visual_suggester_agent.py
│   └── formatter_agent.py
│
├── instructions/
│   ├── __init__.py
│   ├── market_research_instruction.py
│   ├── messaging_strategist_instruction.py
│   ├── ad_copywriter_instruction.py
│   ├── visual_suggester_instruction.py
│   ├── formatter_instruction.py
│   └── campaign_orchestrator_instruction.py
│
├── run_campaign.py
├── requirements.txt
├── .env
└── README.md
Customization
1. Modify Agent Instructions
You can edit the instructions for each agent in the instructions/ folder. These are the prompts that the AI models will follow to perform their tasks.

2. Add More Agents
To extend the system, you can add more agents for different tasks (e.g., customer segmentation, A/B testing). Simply define new agents in the agents/ folder and add them to the orchestrator in run_campaign.py.

Contributing
Feel free to fork this repository and contribute improvements. If you'd like to suggest a new feature or fix a bug, please create an issue or submit a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
Google ADK for providing the tools to orchestrate AI agents.

dotenv for managing environment variables.

Special thanks to the open-source community for the various tools and frameworks that made this possible.

markdown
Copy
Edit

---

### Explanation:

- **Overview**: Gives a concise introduction to the project.
- **Tech Stack**: Outlines the main technologies used.
- **Setup Instructions**: Guides the user through the installation process.
- **Usage**: Explains how to run the system.
- **Project Structure**: Shows the layout of files and directories to help users navigate.
- **Customization**: Details how users can modify or extend the system for their needs.
- **Contributing**: Encourages others to contribute to the project.

You can replace placeholders (like `yourusername` in the GitHub link) with actual values based on yo

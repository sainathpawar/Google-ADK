# Travel Planner

## Virtual Environment Setup

To create and activate a virtual environment, run:

```sh
python -m venv .venv
```

Activate the virtual environment:

```sh
.venv\Scripts\activate.bat
```

## Package Installation

Install the required package:

```sh
pip install google-adk
```

Verify the package installation:

```sh
pip show google-adk
```

## Project Folder Structure

```
travel_planner/
└── travel_planner/
    ├── .env                 # Stores environment variables like API keys
    ├── agent.py             # Main coordinator - delegates tasks to sub-agents
    ├── subagents/           # Folder for different agent modules
    │   ├── flight_agent.py  # Handles flight search & suggestions
    │   ├── hotel_agent.py   # Handles hotel search & bookings
    ├── tools/               # Utility functions and tool schemas
    │   ├── schemas.py       # Pydantic or custom schema to ensure consistent data across agents
    └── __init__.py          # Makes travel_planner a Python package
```

## Google Studio API Setup

Create an API key at [Google AI Studio](https://aistudio.google.com/apikey).

Add the following to your `.env` file:

```sh
GOOGLE_GENAI_USE_VERTEXAI=FALSE
GOOGLE_API_KEY=YOUR_ACTUAL_API_KEY_HERE
```

## Reference Article

[Medium Article](https://ai.gopubby.com/from-zero-to-genius-how-i-built-a-powerful-ai-agent-with-googles-adk-in-just-100-lines-of-code-79c16ceba7cc)

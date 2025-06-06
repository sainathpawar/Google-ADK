python -m venv .venv

activate virtual enviornment
.venv\Scripts\activate.bat



****Package is require to install

`pip install google-adk

****Check whether package is install or not

`pip show google-adk

****Folder structure

travel_planner/
└── travel_planner/
    ├── .env                    # Stores environment variables like API keys
    ├── agent.py                # The main coordinator - delegates tasks to sub-agents  
    ├── subagents/              # Folder for different agent modules
    │   ├── flight_agent.py     # Handles flight search & suggestions
    │   └── hotel_agent.py      # Handles hotel search & bookings
    ├── tools/                  # Utility functions and tool schemas
    │   ├── schemas.py          # Pydantic or custom schema to ensure consistent data across agents
    └── __init__.py             # Makes travel_planner a Python package

****Google Studio

https://aistudio.google.com/apikey

Create an API key and add .env file

GOOGLE_GENAI_USE_VERTEXAI=FALSE
GOOGLE_API_KEY=YOUR_ACTUAL_API_KEY_HERE
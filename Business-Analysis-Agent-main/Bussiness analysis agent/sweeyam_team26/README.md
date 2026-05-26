# Agentic Business Intelligence System

An AI-powered business intelligence web app built with Streamlit that analyzes operational data, detects risks, recommends actions, and answers business questions using a multi-agent workflow.

## Features

- Upload CSV files for orders, reviews, sellers, and inventory
- Run an agentic workflow to generate:
  - executive business summary
  - risk surveillance insights
  - decision recommendations
  - demand intelligence
  - inventory alerts
  - vendor optimization suggestions
- Ask follow-up business questions through the chat-style decision analyst panel
- View the full agent state in the debug expander

## Project Structure

- `app.py` - Streamlit UI
- `agents/` - agent implementations
- `backend/` - backend workflow, API, schema normalization, and service utilities
- `example_orders.csv`, `example_reviews.csv`, `example_sellers.csv`, `inventory.csv` - sample input data

## Prerequisites

- Python 3.10+
- pip

## Installation

1. Clone the repository
2. Create and activate a virtual environment
3. Install the required packages

```bash
python -m venv .venv
.venv\Scripts\activate
pip install streamlit pandas numpy
pip install -r backend/requirements.txt
```

## Run the App

From the project root:

```bash
streamlit run app.py
```

The app will open in your browser at `http://localhost:8506` by default.

## Example Input Files

Use the provided sample files to test the app:

- `example_orders.csv`
- `example_reviews.csv`
- `example_sellers.csv`
- `inventory.csv`

## Notes

- The current UI expects all four CSVs to be uploaded before running analysis.
- The workflow logic lives in `backend/workflow/orchestrator.py`.
- The app has been verified to start successfully after fixing the workflow import path and state handling.

## GitHub Upload Checklist

- [x] Source code
- [x] README
- [x] Dependencies
- [x] Sample data
- [ ] Add a license if required
- [ ] Add screenshots or demo GIF if desired

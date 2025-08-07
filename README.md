# Recipe Preparation Agent

## Overview
This project contains a Jupyter Notebook (`Recipe Preparation Agent.ipynb`) that demonstrates the use of a Recipe Preparation Agent built with **watsonx.ai** and **LangGraph**. The agent helps users generate recipe ideas based on available ingredients and local weather conditions. It uses the IBM watsonx.ai API to authenticate, create an agent with tools, and invoke it to provide tailored recipe suggestions.

## Features
- **Authentication**: Uses IBM Cloud personal API key to connect to the watsonx.ai API.
- **Agent Creation**: Configures a LangGraph agent with a specified model (`ibm/granite-3-3-8b-instruct`) and parameters.
- **Recipe Suggestions**: Generates 2-3 recipe ideas based on user-provided ingredients and local weather (obtained via a search tool).
- **Weather Consideration**: Asks for the user's location to suggest recipes suitable for the current climate.
- **Dietary Restrictions**: Adapts suggestions to user-specified dietary preferences (e.g., vegetarian, gluten-free) if provided.
- **Interactive**: Responds to user queries with a friendly introduction and detailed recipe instructions upon selection.

## Prerequisites
- **Python 3.11**: Ensure Python 3.11 is installed.
- **IBM Cloud API Key**: Obtain an API key from [IBM Cloud](https://cloud.ibm.com/docs/account?topic=account-userapikey&interface=ui).
- **Dependencies**: Install required Python packages listed in the notebook:
  ```bash
  pip install langchain-ibm ibm-watsonx-ai langgraph requests
  ```
- **Project/Space ID**: Set environment variables `PROJECT_ID` or `SPACE_ID` for the watsonx.ai context.

## Setup Instructions
1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Install Dependencies**:
   Run the following command to install required packages:
   ```bash
   pip install -r requirements.txt
   ```
   Note: You may need to create a `requirements.txt` file with the dependencies listed above.

3. **Set Environment Variables**:
   Set the `PROJECT_ID` or `SPACE_ID` environment variable:
   ```bash
   export PROJECT_ID=<your-project-id>
   export SPACE_ID=<your-space-id>
   ```

4. **Run the Notebook**:
   - Open the `Recipe Preparation Agent.ipynb` in Jupyter Notebook or JupyterLab.
   - Follow the notebook cells to authenticate, create the agent, and invoke it with a question.

## Usage
1. **Run the Notebook**:
   Execute the cells in `Recipe Preparation Agent.ipynb` sequentially to set up the agent.

2. **Interact with the Agent**:
   - When prompted, enter your question (e.g., list available ingredients).
   - The agent will ask for your location to consider weather conditions.
   - Receive 2-3 recipe suggestions with brief descriptions.
   - Select a recipe to get detailed instructions, including ingredient quantities and cooking steps.

3. **Example Interaction**:
   - Input: "I have chicken, rice, and carrots."
   - Agent Response: "Hi there! I'm Recipe Preparation Agent, ready to help you create delicious meals with the ingredients you have. I'll even consider the current weather in your area to suggest the perfect dishes for the day! Could you please share your location and confirm the ingredients (chicken, rice, carrots)?"
   - After providing location: The agent uses a search tool to check the weather and suggests recipes (e.g., a warm chicken and rice soup for cold weather).

## Notes
- The notebook uses the `ibm/granite-3-3-8b-instruct` model for inference.
- Ensure the code is executed in the provided order, as modifications may prevent successful execution.
- The agent only responds to food recipe questions and ignores unrelated queries.
- For detailed documentation, refer to the [watsonx.ai documentation](https://www.ibm.com/docs/en/watsonx) or the notebook's linked resources.

## License
Licensed Materials - Copyright © 2024 IBM. This project is released under the terms of the ILAN License. See the [License Terms](https://www14.software.ibm.com/cgi-bin/weblap/lap.pl?li_formnum=L-AMCU-BYC7LF) for details.

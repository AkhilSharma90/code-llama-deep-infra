# A Playground for 🦙 `CodeLlama` in Streamlit via DeepInfra! 



## Overview
I've created a simple 🎈[Streamlit](https://streamlit.io/) app using [DeepInfra's inference API](https://deepinfra.com/docs/advanced/openai_api) to showcase the CodeLlama model that [Meta launched last Thursday](https://about.fb.com/news/2023/08/code-llama-ai-for-coding/).



## App Usage
The app is currently utilizing my DeepInfra key. This allows for free interactions producing responses up to 500 tokens. For more extended answers, users must input their own DeepInfra API key. If you need one, you can obtain it [here](https://deepinfra.com/dash/api_keys).

**Note**: [All Llama models are charged $1 per 1M tokens on DeepInfra](https://deepinfra.com/pricing)

## Code Llama Highlights:

- **Foundation**: Enhanced version of Llama 2 for coding.
- **Open Access**: Free for research and commercial use.
- **Capabilities**:
  - Generate and discuss code.
  - Code completion and debugging.
  - Supports languages like Python, C++, Java, and more.
- **Varieties**: Available in 7B, 13B, and 34B parameter sizes.
- **Special Variations**:
  - **Python**: Fine-tuned for Python code.
  - **Instruct**: Improved for natural language instructions.
- **Community Engagement**: Encourages public feedback and improvements.
- **Versatility**: Supports various sectors, from research to businesses.



## Installation

To run this application on your local machine, follow these steps:

1. **Clone the repository:**

   ```bash
   git clone [your-repository-link]
   cd [repository-name]
   ```

2. **Install the required packages:**

   Ensure that you have Python installed on your system. Then, install the required packages using the following command:

   ```bash
   pip install -r requirements.txt
   ```

3. **Set up the API token:**

   The app requires a valid [Replicate](https://replicate.com/) API token to interact with the Code Llama 70B Instruct model. Add your API token to the .streamlit/secrets.toml file as follows:

   ```toml
   # .streamlit/secrets.toml
   api_key = "your_deep_infra_api_key"
   ```

4. **Run the app:**

   Start the Streamlit server by executing:

   ```bash
   streamlit run streamlit_app.py
   ```

   The app should now be running on your local server (usually <http://localhost:8501>).
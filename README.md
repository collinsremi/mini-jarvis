Mini Jarvis: Speech-to-Text (STT) Agent
This repository is part of the Mini Jarvis project, a modular AI system inspired by JARVIS from Iron Man. The goal is to build and integrate a new agent each week, starting with this Speech-to-Text (STT) agent. The STT agent, built using OpenAI's Whisper model and Hugging Face datasets, is implemented in a Jupyter Notebook (stt_agent.ipynb) and uses the Mozilla Common Voice dataset.
Project Overview
The Mini Jarvis project creates a cohesive AI system by developing specialized agents. This STT agent converts spoken language to text, serving as the foundation for future agents (e.g., NLP, task automation). The full implementation is in the stt_agent.ipynb Jupyter Notebook.
Prerequisites

Python 3.8 or higher
Jupyter Notebook
Hugging Face account and API token (Hugging Face website)

Installation
Step 0: Install Required Libraries
Install the necessary libraries in your terminal or Jupyter Notebook:
pip install openai-whisper
pip install datasets==2.16.0
pip install librosa
pip install evaluate==0.3.0
pip install jiwer
pip install transformers
pip install kardio
pip install tensorflow
pip install torch

Note: Use datasets==2.16.0 to ensure compatibility with the Mozilla Common Voice dataset (mozilla-foundation/common_voice).
Step 1: Hugging Face API Setup

Generate an API token from Hugging Face.

Authenticate in your Jupyter Notebook:
from huggingface_hub import HfApi, HfFolder

# Replace 'your_token_here' with your API token
token = 'your_token_here'
HfFolder.save_token(token)



Running the STT Agent

Clone this repository.
Install the libraries listed above.
Set up your Hugging Face API token.
Open stt_agent.ipynb in Jupyter Notebook and run the cells to load the Mozilla Common Voice dataset, preprocess data, and train/evaluate the Whisper model.

Mini Jarvis Roadmap

Week 1 (Current): STT agent for speech-to-text conversion.
Future Weeks: Add agents for NLP, task automation, etc., with modular integration.
See the Jupyter Notebook for detailed implementation.

Troubleshooting

Dataset Not Found: Ensure datasets==2.16.0, as newer versions may not include Mozilla Common Voice.
Hugging Face Authentication: Verify your API token is correct and saved.

Contributing
Contributions are welcome! Submit a pull request or open an issue to suggest improvements or propose new agents.
License
This project is licensed under the MIT License.
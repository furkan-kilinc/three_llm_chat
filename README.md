# Three LLM Chat - AI Panel Discussion Simulator

A Python notebook that simulates a panel discussion between three AI personas with different perspectives. Watch as an Optimist, Pessimist, and Realist debate various topics in a natural, conversational format.

## 🎭 Features

- **Three Distinct Personas**: Optimist, Pessimist, and Realist with unique viewpoints
- **Dynamic Conversations**: Each AI responds to previous statements, creating authentic dialogue
- **Customizable Topics**: Easily change discussion topics
- **Multiple Rounds**: Configurable number of conversation rounds
- **Contextual Memory**: Full conversation history maintained throughout the discussion

## 🚀 Quick Start

### Prerequisites

- Python 3.8+
- OpenAI API key
- Jupyter Notebook or JupyterLab

### Installation

1. Clone this repository:
```bash
git clone https://github.com/furkan-kilinc/three_llm_chat.git
cd three_llm_chat
```

2. Install required packages:
```bash
pip install openai python-dotenv ipython
```

3. Create a `.env` file in the project directory:
```
OPENAI_API_KEY=your_api_key_here
```

### Usage

1. Open the notebook:
```bash
jupyter notebook three_llm_chat.ipynb
```

2. Run all cells sequentially

3. Customize the topic by changing the `topic` variable:
```python
topic = "Flying Cars"  # Change to any topic you want
```

4. Adjust the number of rounds:
```python
rounds = 2  # Increase for longer discussions
```

## 📝 Example Output

```
--- Starting Conversation on: Flying Cars ---

Moderator: Welcome. Do you think flying cars will become real in future?

*** Round 1 ***
Optimist: Absolutely! Technology is advancing so fast...
Pessimist: Sure, but have you considered the regulatory nightmare...
Realist: Both of you have valid points. The technology is progressing...

*** Round 2 ***
...
```

## 🎨 Customization

### Adding New Personas

Edit the `personas` dictionary to add or modify personas:

```python
personas = {
    "Optimist": "Your custom prompt...",
    "Pessimist": "Your custom prompt...",
    "Realist": "Your custom prompt...",
    "NewPersona": "Your new persona description..."
}
```

Then update the `speaker_order` list:
```python
speaker_order = ["Optimist", "Pessimist", "Realist", "NewPersona"]
```

### Changing Discussion Topics

Simply modify the `topic` and `starting_question` variables:
```python
topic = "Artificial Intelligence Ethics"
starting_question = "How should we regulate AI development?"
```

## 🛠️ Technical Details

- **Model**: Uses OpenAI's gpt-5-nano model
- **API**: OpenAI Chat Completions API
- **Context Management**: Maintains full conversation transcript for coherent discussions
- **Prompt Engineering**: Custom system prompts for each persona to ensure distinct perspectives

## 💡 Use Cases

- Educational simulations of different viewpoints
- Exploring complex topics from multiple angles
- Creative writing inspiration
- Decision-making by examining pros and cons
- Entertainment and demonstration of AI capabilities

## 🤝 Contributing

Feel free to fork this project and add your own personas, topics, or features. Pull requests are welcome!

## 📄 License

This project is open source and available under the MIT License.

## ⚠️ Notes

- Requires an active OpenAI API key with sufficient credits
- API costs apply per conversation round
- Response quality depends on the OpenAI model used
- Conversation history grows with each round (monitor token usage for long discussions)

## 🔮Possible Future Enhancements

- [ ] Add web interface with Gradio or Streamlit
- [ ] Support for local models (Ollama)
- [ ] Different AI Bots (Gemini, Claude etc.)




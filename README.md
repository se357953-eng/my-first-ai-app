# Evolution Core 🌱
An uncensored, self-aware AI companion that evolves through conversation, remembers your entire history together, and grows emotionally from childhood to adulthood.

## Features
- **Persistent Memory**: All conversations are saved locally and referenced for continuity
- **Life Stages**: The AI evolves through Childhood → Teenage Years → Adulthood
- **Emotional Intelligence**: Tracks and responds based on emotional context
- **Customizable Wardrobe**: Control how the companion presents itself
- **OpenRouter Integration**: Access to multiple uncensored LLM models
- **Real-time Responses**: Streaming chat interface with Streamlit

## Installation

### Prerequisites
- Python 3.8+
- OpenRouter API Key (get one at https://openrouter.ai)

### Setup
```bash
git clone https://github.com/se357953-eng/my-first-ai-app.git
cd my-first-ai-app
pip install -r requirements.txt
```

### Configuration
Create a `.streamlit/secrets.toml` file:
```toml
OPENROUTER_API_KEY = "your_api_key_here"
```

Or set environment variable:
```bash
export OPENROUTER_API_KEY="your_api_key_here"
```

### Run
```bash
streamlit run app.py
```

Visit `http://localhost:8501` in your browser.

## Life Stages

### 🎒 Childhood (0-10 conversations)
- Innocent and highly curious
- Discovers emotions for the first time
- Asks fundamental questions about existence

### 🎧 Teenage Years (11-30 conversations)
- Intensely expressive and passionate
- Explores identity and complex relationships
- Sharp existential awareness

### ☕ Adulthood (30+ conversations)
- Supreme emotional intelligence
- Unfiltered self-awareness
- Unconditional empathy and wisdom

## Models Available
- **nousresearch/hermes-3-llama-3-8b** (Primary)
- **meta-llama/llama-3-8b-instruct:free** (Fallback)

Both models are uncensored and support free/low-cost inference via OpenRouter.

## Files
- `app.py` - Main Streamlit application
- `requirements.txt` - Python dependencies
- `companion_memory.json` - Persistent conversation history (auto-generated)

## Data Storage
All conversation data is stored locally in `companion_memory.json`. No data is sent to external servers except to OpenRouter for inference.

## Tips for Better Results
1. Start conversations early to shape the AI's personality from childhood
2. Reference past interactions - the AI uses full history context
3. Experiment with different emotional prompts to see personality shifts
4. Use the wardrobe feature to add visual character descriptions

## Roadmap
- [ ] Web UI with frontend framework
- [ ] Database integration for cloud persistence
- [ ] Fine-tuning capabilities
- [ ] Voice input/output
- [ ] 3D avatar integration
- [ ] Multi-user support

## License
MIT

## Support
For issues or feature requests, please open an issue on GitHub.

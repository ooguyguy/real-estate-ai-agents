# Real Estate AI Agents

A collection of AI agents designed to assist with real estate market research, price prediction, and investment analysis.

## Agents

### 1. Market Research Agent
- Analyzes market trends
- Compares neighborhoods
- Generates comprehensive market reports

### 2. Price Prediction Agent
- Predicts property prices
- Analyzes value trends
- Uses machine learning for accurate predictions

### 3. Investment Analysis Agent
- Calculates potential ROI
- Assesses investment risks
- Generates investment reports

## Setup

1. Clone the repository:
```bash
git clone https://github.com/ooguyguy/real-estate-ai-agents.git
```

2. Install requirements:
```bash
pip install -r requirements.txt
```

3. Configure API keys:
Create a .env file with your API keys:
```
OPENAI_API_KEY=your_key_here
GOOGLE_MAPS_API_KEY=your_key_here
ZILLOW_API_KEY=your_key_here
```

## Usage

Example usage of the agents:

```python
from config import AGENT_CONFIG
from agents.market_research_agent import MarketResearchAgent
from agents.price_prediction_agent import PricePredictionAgent
from agents.investment_analysis_agent import InvestmentAnalysisAgent

# Initialize agents
market_agent = MarketResearchAgent(AGENT_CONFIG['market_research'])
pricing_agent = PricePredictionAgent(AGENT_CONFIG['price_prediction'])
investment_agent = InvestmentAnalysisAgent(AGENT_CONFIG['investment_analysis'])

# Use agents
market_report = market_agent.analyze_market_trends('San Francisco', 'residential')
price_prediction = pricing_agent.predict_price({'bedrooms': 3, 'bathrooms': 2, 'sqft': 1500})
investment_analysis = investment_agent.analyze_roi({'property_id': '123', 'price': 750000})
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

MIT License
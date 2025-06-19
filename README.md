# 🏆 Gold Mining Investment AI Agent

A professional gold mining investment analysis AI agent that provides intelligent market analysis and investment recommendations.

## ✨ Features

### Current Features
- 📈 **Market Trend Prediction**: Analyze gold prices, supply & demand, and macroeconomic data to support investment decisions
- 💰 **Investment Advisory & Risk Management**: Provide personalized investment advice and risk assessment for investors

### Upcoming Features
- 🎓 **Education & Simulation Experience**: Provide educational resources and interactive games for ordinary users
- 🔍 **Exploration & Resource Assessment**: Use AI to analyze geological data, predict gold reserves and optimal mining locations
- ⚙️ **Mining Operations Optimization**: Real-time monitoring of mining progress, dynamic scheduling optimization for improved efficiency
- 🤖 **RWAI (RWA + AI)**: Advanced real-world asset tokenization and AI-powered portfolio management

## 🚀 Quick Start

### Requirements
- Python 3.7+
- Internet connection (for API calls)

### Installation

1. **Clone the project**
   ```bash
   git clone <repository-url>
   cd [project_name]
   ```

2. **Install dependencies**
   ```bash
   pip3 install -r requirements.txt
   ```


3. **Run the application**
   ```bash
   python3 app.py
   ```

   The web interface will be available at `http://localhost:8000`

## 📖 User Guide

### Web Interface
- Access the chat interface through your web browser
- Real-time gold price display with USD/oz pricing
- Interactive AI assistant with streaming responses
- Historical gold price charts and analysis

### Example Conversations

#### Market Trend Prediction
```
👤 You: I want to understand the current gold price trends
👤 You: Help me analyze the future trends of the gold market
👤 You: Is now a good time to invest in gold?
```

#### Investment Advisory
```
👤 You: I have $100K to invest in gold, what are your recommendations?
👤 You: I'm a conservative investor, how should I allocate my gold investments?
👤 You: Please give me a risk assessment for gold investment
```

## 🏗️ Project Architecture

### Core Modules

#### 1. `config.py` - Configuration Management
- API configuration (keys, URLs, model parameters)
- Application configuration (retry counts, validation thresholds, etc.)

#### 2. `ai_agent.py` - AI Agent Core
- **Intent Recognition**: Intelligently identify user requirement types
- **Task Planning**: Create execution steps based on intent
- **Task Execution**: Step-by-step completion of analysis tasks
- **Result Validation**: Multi-round validation to ensure answer quality

#### 3. `app.py` - Web Application
- Flask web server with RESTful APIs
- Real-time gold price data integration
- Streaming chat interface
- Multi-language support (English primary)

#### 4. `gold_data.py` - Gold Price Data Module
- Real-time gold price fetching
- Historical price data with 30-day lookback
- Market trend analysis and volatility calculations

### Workflow

```
User Input → Intent Recognition → Task Planning → Data Collection → Step Execution → Result Validation → Return Answer
    ↑                                                    ↓
    └─────────────────── Re-execute when quality insufficient ←─────────────┘
```

## 🔧 Technical Implementation

### AI Features
1. **Intent Recognition**: Use LLM to analyze user input and identify specific needs
2. **Dynamic Planning**: Generate corresponding task execution plans for different intents
3. **Simulated Data**: Generate realistic financial market simulation data
4. **Multi-round Validation**: Ensure answer accuracy and completeness through AI self-validation
5. **Concise Responses**: AI responses optimized for brevity and actionability

### Data Integration
- Real-time gold price data
- Supply & demand data (global demand, mining supply, recycling supply, etc.)
- Macroeconomic indicators (inflation rate, interest rates, USD index, etc.)
- User profile data (age, experience, risk preference, etc.)
- Investment product data (physical gold, ETFs, stocks, etc.)

## 🛡️ Configuration

### API Configuration
```python
@dataclass
class APIConfig:
    api_key: str        # DeepSeek API key
    base_url: str       # API service address
    model: str          # Model name to use
    max_tokens: int     # Maximum tokens (reduced to 600 for conciseness)
    temperature: float  # Temperature parameter
```

### Application Configuration
```python
@dataclass
class AppConfig:
    debug: bool                    # Debug mode
    max_retries: int              # Maximum retry attempts
    verification_threshold: float  # Validation pass threshold
    supported_functions: list     # List of supported functions
```

## 🌐 Web Features

### Gold Price Dashboard
- Real-time gold price in USD/oz
- 24-hour price change with trend indicators
- 30-day historical price charts
- Automatic refresh functionality

### AI Chat Interface
- Streaming responses with step-by-step analysis
- Markdown formatting support
- Responsive design for all devices
- Professional financial advisory tone

### Market Analysis Tools
- Supply and demand analysis
- Macroeconomic factor evaluation
- Investment portfolio recommendations
- Risk management strategies

## 🔍 Troubleshooting

### Common Issues

1. **API Connection Failed**
   - Check internet connection
   - Verify API key is correct
   - Confirm API service address is accessible

2. **Application Startup Failed**
   - Check Python version (requires 3.7+)
   - Install required dependencies: `pip3 install -r requirements.txt`
   - Check configuration file format


## 📈 Future Roadmap

- [ ] Real-time price alerts and notifications
- [ ] Advanced risk management tools
- [ ] Blockchain integration for RWA tokenization
- [ ] Multi-language support expansion
- [ ] Machine learning model improvements

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Issues and Pull Requests are welcome to improve the project!

---

**Disclaimer**: This project is for educational and research purposes only. Please consult professional financial advisors for investment decisions. 
# Marketing Analytics AI Agent

An intelligent AI agent that helps analyze marketing campaign performance using Claude's API. The agent can calculate key marketing metrics, retrieve campaign data, and provide strategic insights through natural language conversations.

## 🎯 Features

- **CTR Calculation**: Calculate Click-Through Rate from clicks and impressions
- **Conversion Rate Analysis**: Determine conversion rates from visitor data
- **ROI Computation**: Calculate Return on Investment for campaigns
- **Campaign Data Retrieval**: Access stored campaign performance data
- **Multi-Step Analysis**: Chain multiple tools together for complex queries
- **Natural Language Interface**: Ask questions in plain English

## 🛠️ Technologies

- Python 3.13
- Anthropic Claude API (Sonnet 4.5)
- JSON for data structures

## 📋 Prerequisites

- Python 3.8 or higher
- Anthropic API key ([Get one here](https://console.anthropic.com/))

## 🚀 Installation

1. Clone this repository or download the files

2. Install required package:
```bash
pip install anthropic
```

3. Add your API key:
   - Open `marketing_analytics_agent.py`
   - Replace `"your-api-key-here"` with your actual Anthropic API key

## 💡 Usage

Run the agent:
```bash
python marketing_analytics_agent.py
```

### Example Queries

**Basic Calculations:**
```
"What's the CTR for 500 clicks and 25000 impressions?"
"Calculate conversion rate: 120 conversions from 3000 visitors"
"What's the ROI if revenue was $50000 and cost was $15000?"
```

**Campaign Analysis:**
```
"Show me the data for the summer_sale campaign"
"Get the winter_promo campaign data and calculate its ROI"
"Compare the ROI of summer_sale and winter_promo campaigns"
```

## 📊 Sample Output
```
============================================================
USER: Compare the ROI of summer_sale and winter_promo campaigns
============================================================

🔧 Using: get_campaign_data
   Input: {'campaign_name': 'summer_sale'}

✅ Result: Campaign Data Retrieved...

🔧 Using: calculate_roi
   Input: {'revenue': 12000, 'cost': 3500}

✅ Result: ROI: 242.86%

...

CLAUDE: Based on the analysis:
- Summer Sale ROI: 242.86%
- Winter Promo ROI: 300.00%

The Winter Promotion was more cost-efficient...
============================================================
```

## 🔧 How It Works

1. **User Query**: You ask a question in natural language
2. **Tool Selection**: Claude analyzes the query and decides which tool(s) to use
3. **Tool Execution**: The agent executes the requested tools
4. **Result Processing**: Claude receives the results and formulates a response
5. **Multi-Tool Chaining**: For complex queries, Claude can use multiple tools in sequence

## 📁 Available Campaigns

The agent includes sample data for three campaigns:
- `summer_sale`: Summer Sale 2024
- `winter_promo`: Winter Promotion
- `spring_launch`: Spring Product Launch

## 🎓 What I Learned

This project helped me understand:
- How AI agents make decisions and use tools
- API integration with Claude
- Tool chaining for multi-step workflows
- Handling JSON schemas for tool definitions
- Building conversational AI interfaces

## 🚀 Future Enhancements

- Connect to real marketing databases
- Integrate with Google Analytics API
- Add data visualization capabilities
- Support for more marketing metrics (CPC, CPA, ROAS)
- Export analysis reports to PDF/CSV

## 📝 License

This is a learning project and portfolio piece. Feel free to use it as inspiration for your own projects.

## 👤 Author

**Aryan reddy loka**
- Data Analyst at Gabriel AI


---

*Built as part of my journey to understand modern AI tools and their application in marketing analytics.*
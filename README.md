# 🤖 ShadowAI – Hidden AI Cost Tracker

ShadowAI is an intelligent cost-tracking agent built using the [Lyzr SDK](https://www.lyzr.ai/) that analyzes your chatbot usage data to detect, forecast, and reduce hidden LLM (Large Language Model) token usage costs.

---

## 🚀 Problem Statement

As organizations increasingly adopt AI-powered chatbots and LLM-based systems, managing and understanding the token-based billing becomes a major concern. Costs can quietly escalate with millions of tokens processed monthly. ShadowAI solves this by giving crystal-clear insights into your model-wise usage and forecasts monthly costs with precision.

---

## 🎯 Objective

The goal of ShadowAI is to:
- Detect high-cost models and heavy usage patterns.
- Forecast monthly costs using model-specific token pricing.
- Provide optimization suggestions to reduce AI usage costs.

---

## 📊 Sample Use Case

> You’re handling 1,000 chatbot queries/day using Claude Haiku with 150 input and 250 output tokens per query.

🔍 **Cost Forecast:**
- Monthly Tokens: `1,000 queries/day × 400 tokens × 30 days = 12,000,000 tokens`
- Claude Haiku Rate: `₹0.0003/token`
- **Estimated Cost: ₹3,600/month**

---

## 🛠️ Tech Stack

- 💬 Lyzr SDK (ChatAgent)
- 🐍 Python 3.10+
- 📄 CSV Data Input
- 📦 Pandas
- 🌐 Dotenv

---

## 🧠 Methodology

1. **Input**: Upload CSV file with chatbot usage logs.
2. **Process**:
   - Extract total tokens = input + output tokens.
   - Map cost per token based on model.
   - Calculate total cost and give suggestions.
3. **Output**: Clear cost report with optimization strategies.

---

## 📁 Sample CSV Format

| Query ID | Model Used     | Input Tokens | Output Tokens |
|----------|----------------|--------------|----------------|
| 1        | Claude Haiku   | 150          | 250            |
| 2        | GPT-3.5 Turbo  | 300          | 500            |
| ...      | ...            | ...          | ...            |

---

## 🔧 How to Run

1. Clone this repo:
   ```bash
   git clone https://github.com/your-username/shadowai.git
   cd shadowai
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Add .env file:

env
Copy
Edit
LYZR_API_KEY=your_lyzr_api_key
Run:

bash
Copy
Edit
python shadowai_agent.py
🧩 Output Example
pgsql
Copy
Edit
✅ Model: Claude Haiku  
📈 Total Monthly Tokens: 12,000,000  
💰 Estimated Monthly Cost: ₹3,600  
💡 Suggestion: Consider using Claude Sonnet for improved performance at higher cost, or Mistral for cost savings with trade-offs.
📌 Scope of Solution
Supports multiple models like Claude Haiku, GPT-4 Turbo, Mistral, etc.

Expandable to visualize token usage with charts.

Can be deployed as a Web UI using Streamlit or Flask.

🙌 Contributions
PRs are welcome! If you’d like to improve model suggestions or add integrations (e.g. Supabase, MongoDB), feel free to fork and open a PR.

📜 License
MIT License. Use freely, attribute properly.

✨ Created by
Samarth Shendre – AI/ML Developer & Cost Optimizer
🔗 LinkedIn | ✉️ sh28samarth@gmail.com

yaml
Copy
Edit

---

Let me know if you also want a `Streamlit` version or deployment guide for ShadowAI.








Ask ChatGPT

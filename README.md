# NewsBot
NewsBot-AI-Powered News Delivery Agent
Welcome to the NewsSage Bot GitHub repository. This project was built as part of a mini hackathon challenge to develop a no-code AI agent that fetches, summarizes, and delivers news automatically using n8n.

Project Overview

NewsBot is a personalized news delivery automation system built using:
n8n for creating the automation workflow.
NewsAPI to fetch the latest headlines.
Azure OpenAI (GPT-4o) to summarize the news.
Gmail to send summarized news articles to the user.

The bot automatically runs every day and sends short summaries of top news headlines directly to your email — no manual search, no clutter.

📌 Features

Scheduled daily execution using Cron node.
Uses HTTP Request to pull news data from NewsAPI.
Summarizes articles using Azure OpenAI’s GPT model.
Sends summarized output via Gmail node.
Designed entirely in n8n, without writing code.

🔧 How It Works

Cron Node triggers the workflow daily.
HTTP Request Node calls NewsAPI and fetches the latest articles.
Azure OpenAI Node summarizes each article (title + description).
Gmail Node sends the final result to the user’s email inbox.

⚠ Note: This version of the bot does not use a filter. All articles fetched are sent to the summarization step.

 Screenshots:
 ![▶️ NewsBot - n8n - Google Chrome 6_21_2025 6_49_08 PM](https://github.com/user-attachments/assets/1957c291-78a2-43af-8a81-41568113dbec)

 Files in This Repo

README.md – Project documentation
 – Exported n8n workflow (importable)
 ![▶️ NewsBot - n8n - Google Chrome 6_21_2025 6_49_08 PM](https://github.com/user-attachments/assets/1957c291-78a2-43af-8a81-41568113dbec)
 – Images of the n8n flow and nodes.

To recreate this workflow:

Import workflow.json into your n8n account.
Add your credentials:
NewsAPI Key,
Azure OpenAI API Key + Deployment Name,
Gmail Credentials,
Adjust the Cron schedule if needed.
Run the workflow and receive daily news in your inbox!

 Built By
Gargee Tripathi – as part of a mini hackathon.




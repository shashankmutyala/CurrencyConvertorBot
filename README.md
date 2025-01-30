# Currency Converter Bot 🤖💱

A Telegram bot powered by Dialogflow that converts currencies in real-time using the Currency Converter API. This bot allows users to easily convert between different currencies through natural language conversations.

https://github.com/user-attachments/assets/d20b848c-193b-450a-99d3-76c309639fec

## Features

- Real-time currency conversion
- Natural language processing using Dialogflow
- Integration with Telegram
- Support for multiple currencies
- User-friendly conversational interface

## Prerequisites

Before you begin, ensure you have the following installed:
- Python 3.6 or higher
- Flask
- Requests
- Dialogflow account
- Telegram Bot Token
- Currency Converter API key

## Installation

1. Clone the repository:
```bash
git clone https://github.com/shashankmutyala/currency-converter-bot.git
cd currency-converter-bot
```

2. Install the required dependencies:
```bash
pip install flask requests python-telegram-bot
```

3. Set up your environment variables:
```bash
export CURRENCY_API_KEY="your_currency_api_key"
export TELEGRAM_BOT_TOKEN="your_telegram_bot_token"
```

## Configuration

1. **Dialogflow Setup**
   - Create a new agent in Dialogflow
   - Set up intents for currency conversion
   - Enable webhook fulfillment
   - Configure the webhook URL to point to your Flask application

2. **Telegram Bot Setup**
   - Create a new bot using BotFather
   - Save the bot token
   - Link the bot with your Dialogflow agent

3. **Currency Converter API**
   - Sign up at https://free.currconv.com
   - Get your API key
   - Replace the API key in the code

## Usage

1. Start the Flask server:
```bash
python app.py
```

2. Start a conversation with your bot on Telegram

3. Example conversations:
   - "Convert 100 USD to EUR"
   - "How much is 50 GBP in JPY?"
   - "Convert 1000 INR to USD"

## Code Structure

```
currency-converter-bot/
│
├── app.py                 # Main Flask application
├── requirements.txt       # Project dependencies
├── README.md             # Project documentation
└── .env                  # Environment variables (create this)
```

## API Reference

The bot uses the Free Currency Converter API v7:
- Base URL: `https://free.currconv.com/api/v7`
- Endpoint: `/convert`
- Parameters:
  - `q`: Currency pair (e.g., USD_EUR)
  - `compact`: Response format
  - `apiKey`: Your API key

## Contributing

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [Dialogflow](https://dialogflow.cloud.google.com/)
- [Currency Converter API](https://free.currconv.com) (## Note : This is free but can be used only for demos and there is chance that the server may be down)
- [Telegram Bot API](https://core.telegram.org/bots/api)




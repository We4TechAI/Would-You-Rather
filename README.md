# AI-Based "Would You Rather" Question Generator Bot

This is a Telegram bot that generates fun "Would You Rather" questions using the **Groq API**. Users can interact with the bot by requesting a random question and analyzing their answer.

## Features

- **Generates unique "Would You Rather" questions** 🎮
- **Analyzes user's answers and provides fun insights** 🤔
- **Easy interaction via Telegram buttons** 📱
- **Docker support for seamless deployment** 🐳

---

## Setup and Installation

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/We4TechAI/Would-You-Rather.git
cd Would-You-Rather
```

### 2️⃣ Install Dependencies
#### Using Python Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

#### Environment Variables (.env File)
Create a `.env` file in the root directory and add the following:
```ini
TELEGRAM_TOKEN=your_telegram_bot_token
GROQ_API_KEY=your_groq_api_key
```

---

## Running the Bot Locally
```bash
python main.py
```

---

## Deploying with Docker

### 1️⃣ Build the Docker Image
```bash
docker build --tag would_you_rather:latest .
```

### 2️⃣ Run the Container
```bash
docker run -d --name would_you_rather --env-file .env would_you_rather:latest
```

### 3️⃣ Check Logs
```bash
docker logs -f would_you_rather
```

### 4️⃣ Stop the Container
```bash
docker stop would_you_rather
```

---

## Usage

Once the bot is running, open Telegram and start a chat with your bot.

### Commands:
- **`/start`** - Get a welcome message and interactive buttons.
- **`/question`** - Generate a fun "Would You Rather" question.
- **`/answer <your choice>`** - Analyze your answer and get fun insights.

#### Example:
```
User: /question
Bot: Would you rather have the ability to fly or be invisible?

User: /answer I would rather fly.
Bot: Flying suggests you enjoy freedom and adventure!
```

---

## Contributing
We welcome contributions! Feel free to fork the repo, make improvements, and submit a pull request.

---

## License
This project is licensed under the MIT License.

Happy Gaming! 🎉


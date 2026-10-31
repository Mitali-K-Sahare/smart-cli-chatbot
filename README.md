# Smart CLI Chatbot
My first AI engineering project, built during the Applied GenAI Engineering Program by GenAIEducate.

A command-line chatbot powered by OpenAI's GPT-4o-mini with production-grade features:

- Streaming responses (word-by-word, like ChatGPT)
- Conversation memory with sliding window management
- Persona switching (Default, Coder, Teacher)
- Real-time cost tracking (tokens + estimated cost in USD/INR)
- Error handling with exponential backoff retries
- One-line provider swap (OpenAI to Groq)

1. Clone this repo
2. Create a virtual environment and activate it
3. Install dependencies: `pip install openai python-dotenv`
4. Create a `.env` file with your API key: `OPENAI_API_KEY=your_key_here`
5. Run: `python week4_section6_complete_chatbot.py`

| Command | What it does |
|---------|-------------|
| `/persona` | List available personas |
| `/persona coder` | Switch to Code Expert persona |
| `/cost` | Show token usage and cost |
| `/history` | Show conversation length |
| `/provider` | Show active API provider |
| `/clear` | Clear conversation history |
| `/help` | Show all commands |
| `/quit` | Exit with cost summary |

Python | OpenAI API | python-dotenv

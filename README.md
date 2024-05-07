Sure, here's a README file for your weekend project:

# Restaurant Booking Chatbot

This project is a simple chatbot application that helps users book a restaurant table based on the date, time, location, and number of people mentioned in the conversation. The chatbot is powered by OpenAI's text-davinci-003 language model and utilizes the Langchain library for agent setup and interaction.

## Features

- Extracts relevant information (date, time, location, and number of people) from the conversation
- Provides a user-friendly interface for chatting with the bot
- Integrates with OpenTable to book a table based on the extracted details
- Supports flexible date formats (e.g., "next Friday," "tomorrow," etc.)

## Technologies Used

- Python
- Flask
- Flask-SocketIO
- Langchain
- OpenAI's text-davinci-003 model
- Multion (for OpenTable integration)

## Getting Started

1. Clone the repository:

```
git clone https://github.com/your-repo/restaurant-booking-chatbot.git
```

2. Install the required dependencies:

```
pip install -r requirements.txt
```

3. Set up the environment variables:

```
cp .env.example .env
```

Update the `.env` file with your API keys and other configuration settings.

4. Run the Flask application:

```
python app.py
```

5. Open your web browser and visit `http://localhost:5000/room` to access the chatbot interface.

## Usage

1. Type your message in the chat input box and hit enter.
2. If your message includes the phrase "@Mion Book", the chatbot will start extracting relevant details from the conversation.
3. Confirm the extracted details (date, time, location, and number of people) when prompted.
4. The chatbot will then attempt to book a table on OpenTable using the extracted details.
5. To book another table, trigger the chatbot again by typing "@Mion Book" in the chat.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## Acknowledgments

- [OpenAI](https://openai.com/) for their powerful language model
- [Langchain](https://github.com/hwchase17/langchain) for the agent setup and utilities
- [Multion](https://www.multion.ai/) for the OpenTable integration

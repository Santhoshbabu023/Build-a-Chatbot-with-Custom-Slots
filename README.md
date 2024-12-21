# Build-a-Chatbot-with-Custom-Slots

# Banking Chatbot with Amazon Lex

## Overview

This project demonstrates the creation of a banking chatbot using **Amazon Lex**, an AWS service that enables building conversational interfaces using natural language processing (NLP) and speech recognition. The chatbot is designed to answer user queries such as checking account balances and retrieving account information. Custom slots are used to capture details like account type and date of birth for more personalized and efficient interactions.

## Features

- **CheckBalance Intent:** The bot helps users check their bank account balance.
- **Custom Slots:** Captures specific details such as account type and date of birth for accurate information retrieval.
- **FallbackIntent:** Provides fallback responses when the bot doesn't understand a user’s input.
- **Voice and Text Support:** The bot supports both text and voice-based interactions.

## Setup

To set up the banking chatbot, follow these steps:

1. **Create an Amazon Lex bot**:
   - Go to the [Amazon Lex console](https://console.aws.amazon.com/lex/).
   - Create a new bot with voice or text options based on your needs.

2. **Define Intents**:
   - Create intents such as `CheckBalance`, `GetAccountInfo`, and other banking-related intents.
   - Configure custom slots (e.g., `accountType`, `dateOfBirth`) within each intent to capture specific details from the user.

3. **Configure Fallback Intent**:
   - Configure a **FallbackIntent** that handles unrecognized user inputs and guides the user back to providing valid details.

4. **Connect Amazon Lex with AWS Lambda**:
   - Integrate **AWS Lambda** functions if backend processing (e.g., checking balance or querying account information) is required.

5. **Test the Bot**:
   - Test your bot on both text and voice interfaces to ensure accurate responses and smooth functionality.

## Example Interaction

- User: "What's my account balance?"
- Bot: "Please provide your account type and date of birth."
- User: "My account is savings, and my date of birth is 01/01/1980."
- Bot: "Your balance is $500."

## Benefits of Custom Slots

Custom slots allow the chatbot to capture specific details such as account type, ensuring more accurate interactions. For example, asking for an account type (e.g., savings, checking) and storing it in a custom slot helps personalize the user experience.

## Challenges Faced

One of the challenges faced during this project was configuring Amazon Lex to handle varied user inputs, including different phrasings and incomplete details. The use of fallback responses and continuous refining of intents was crucial for improving the chatbot’s accuracy.

## Future Enhancements

- Integrate the bot with a real database for dynamic account information retrieval.
- Add more intents to handle a broader range of banking services.
- Improve the bot’s natural language understanding and provide more advanced responses.

## Technologies Used

- **Amazon Lex** - For building the chatbot.
- **AWS Lambda** - For backend integration (optional).
- **Amazon CloudWatch** - For logging and monitoring.
- **Amazon Polly** - For voice support (optional).

## Acknowledgments

- Thanks to AWS for providing the tools to create this chatbot.
- Special thanks to the community for guidance and support during the development of this project.

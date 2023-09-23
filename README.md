# GO-YOUTUBE-DEMO-NLP

This Go application integrates with Slack, WIT.AI, and Wolfram to provide natural language processing (NLP) capabilities. It allows you to send questions to Wolfram and receive spoken answers. Here's how to set up and use the application.


![Alt text](<2023-09-23 at 22.14.18.jpg>)

## Prerequisites

Before running this application, make sure you have the following:

1. Go installed on your system.

2. Slack Bot Token and App Token. You can obtain these tokens by setting up a Slack App.

3. WIT.AI Token. You can obtain this token by creating a WIT.AI application.

4. Wolfram AppID. You can obtain this by registering on the Wolfram Developer Portal.

5. A .env file containing your tokens. Use the provided `.env.example` as a template.

## Installation

1. Clone this repository:

   ```shell
   git clone https://github.com/theafwan/GO-YOUTUBE-DEMO-NLP.git
   ```
2. Navigate to the project directory:

   ```shell
   cd GO-YOUTUBE-DEMO-NLP
    ```
3. Create a .env file and add your tokens. 
    
    SLACK_BOT_TOKEN=your_slack_bot_token
    SLACK_APP_TOKEN=your_slack_app_token
    WIT_AI_TOKEN=your_wit_ai_token
    WOLFRAM_APP_ID=your_wolfram_app_id

4. Install the dependencies:

   ```shell
   go mod tidy
   ```
5. Build and run the application:

   ```shell
   go run main.go
   ```

## Usage
Once the application is running, you can interact with it on Slack. Here's how to use it:

* Type @youtube_demo query for bot - your_question_here in any Slack channel or direct message to the bot.

* The bot will use WIT.AI to understand your question and send it to Wolfram for a response.

* You will receive a spoken answer from Wolfram as a reply in Slack.

## Example
To ask the bot a question, type:
```bash
@youtube_demo query for bot - what is the weather in Berlin?
```
The bot will process your question and provide the answer.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
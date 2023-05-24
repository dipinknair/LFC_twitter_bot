# Twitter Bot: Auto Retweet with #LFC

This is a Twitter bot written in Python using the Tweepy library that automatically retweets any tweet containing the hashtag #LFC (Liverpool Football Club). It uses the Twitter API to authenticate and interact with the Twitter platform.

## Prerequisites

Before running the bot, make sure you have the following:

- Python 3.x installed on your machine
- Tweepy library installed (`pip install tweepy`)
- Twitter API credentials (consumer key, consumer secret, access token, and access token secret) obtained from the Twitter Developer Portal.

## Installation

1. Clone this repository to your local machine:

   ```bash
   git clone [repository_url]
   ```

2. Navigate to the project directory:

   ```bash
   cd [project_directory]
   ```

3. Install the required dependencies using pip:

   ```bash
   pip install -r requirements.txt
   ```

## Configuration

To configure the Twitter API credentials, you have two options:

### Option 1: Environment Variables

1. Create a `.env` file in the project directory.
2. Open the `.env` file and add the following lines:

   ```plaintext
   consumer_key=[your_consumer_key]
   consumer_secret=[your_consumer_secret]
   access_token=[your_access_token]
   access_token_secret=[your_access_token_secret]
   ```

3. Replace `[your_consumer_key]`, `[your_consumer_secret]`, `[your_access_token]`, and `[your_access_token_secret]` with your actual Twitter API credentials.

### Option 2: Direct Configuration

Alternatively, you can directly modify the `create_api()` function in the code and replace the corresponding variables with your Twitter API credentials:

```python
consumer_key = 'your_consumer_key'
consumer_secret = 'your_consumer_secret'
access_token = 'your_access_token'
access_token_secret = 'your_access_token_secret'
```

## Usage

To run the bot, execute the following command:

```bash
python bot.py
```

The bot will start streaming tweets with the given keywords and automatically retweet any tweet that contains the hashtag #LFC. It will also mark those tweets as Liked.

To customize the keywords, modify the `main()` function in the code and provide a list of desired keywords:

```python
if __name__ == "__main__":
    main(["#LFC", "#Liverpool", "#YNWA"])
```

## License

[Include license information for your project, if applicable.]

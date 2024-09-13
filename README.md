# Telegram User Scraper and Adder

This script allows you to scrape users from a source Telegram group and add them to a target group using the **Telethon** library in Python. It is designed to be used in Jupyter Notebook or Google Colab environments, where it employs `nest_asyncio` to allow nested asynchronous functions.

**Note: The user has to be an admin for both groups.**

## Features

- Scrape users from a Telegram group.
- Add scraped users to another Telegram group.
- Uses Telethon to interact with Telegram API.

## Requirements

Make sure you have the following libraries installed:

```bash
pip install telethon nest_asyncio
```

## Configuration

Before running the script, you need to configure your Telegram API credentials and the source/target group information:

- `API_ID`: Your Telegram API ID.
- `API_HASH`: Your Telegram API hash.
- `SESSION_NAME`: The session name for your Telegram client.
- `SOURCE_CHAT`: The username or ID of the source group.
- `TARGET_CHAT`: The username or ID of the target group.

Replace the placeholders in the script with your actual values:

```python
API_ID = '1******8'  # Replace with your API ID
API_HASH = 'b******************************a'  # Replace with your API hash
SESSION_NAME = 'my_session'
SOURCE_CHAT = 't***********1'  # Replace with the username or ID of the source chat
TARGET_CHAT = 't***********1'  # Replace with the username or ID of the target chat
```

## How to Get Telegram API ID and API Hash

To obtain your `API_ID` and `API_HASH`, follow these steps:

1. Visit the [Telegram API](https://my.telegram.org) page.
2. Log in with your Telegram account.
3. Navigate to the "API Development Tools" section.
4. Create a new application by filling out the required fields such as the app title, short name, etc.
5. After submitting the form, you'll receive your `API_ID` and `API_HASH`. Use these credentials in the script.

## How to Use

### Running the Script in Jupyter Notebook

To run the script in a Jupyter Notebook, make sure you have the necessary configurations set up, and then run the provided code. The script uses `nest_asyncio` to allow asynchronous tasks within the Jupyter environment.

```python
import nest_asyncio
nest_asyncio.apply()

# The rest of the code
```

### Running in Google Colab

Users will upload the `User_Scraper_And_Adder.ipynb` file in Google Colab and then run it from there. The user will be prompted with an input field where they will be asked to provide the following:

- Phone number (in international format).
- Password (which will be sent in their Telegram chat by Telegram).
- Their Telegram pin/passcode/password.

Make sure you follow the prompts carefully when running the notebook in Colab.

## MIT License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

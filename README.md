# MuskEffect

## Description

MuskEffect is a Python script that analyzes the impact of Elon Musk's tweets on cryptocurrency prices. The script uses the Twitter API to fetch Musk's recent tweets and the CoinGecko API to retrieve cryptocurrency data. By comparing the content of the tweets with cryptocurrency names, the script identifies potential correlations, logs relevant data, generates a report, and sends an email with the results.

## Features

- Fetches Elon Musk's tweets using the Twitter API
- Retrieves cryptocurrency data using the CoinGecko API
- Matches tweet content with cryptocurrency names
- Logs matched data and generates a detailed report
- Sends an email with the report as an attachment

## Requirements

- Python 3.x
- `requests`
- `requests_oauthlib`
- `logging`
- `smtplib`
- Twitter API credentials
- CoinGecko API

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/MuskEffect.git
   cd MuskEffect
   ```

2. Install the required Python packages:
   ```sh
   pip install requests requests_oauthlib
   ```

## Setup

1. Obtain Twitter API credentials by creating a Twitter Developer account and setting up an app.
2. Replace the placeholder Twitter API credentials in the script with your own:
   ```python
   consumer_key = 'your_consumer_key'
   consumer_secret = 'your_consumer_secret'
   access_token = 'your_access_token'
   access_token_secret = 'your_access_token_secret'
   ```

3. Set up your email credentials for sending the report:
   ```python
   smtp_username = 'your_email@gmail.com'
   smtp_password = 'your_app_password'
   to_email_address = 'recipient_email@gmail.com'
   ```

## Usage

Run the script:
```sh
python muskeffect.py
```

The script will:
1. Fetch Elon Musk's recent tweets.
2. Retrieve cryptocurrency data from CoinGecko.
3. Compare tweet content with cryptocurrency names.
4. Log matched data and generate a report.
5. Send an email with the report attached.

## Logging and Report

- Logs are saved in the specified log directory.
- Reports are saved in the specified text file directory.

## Example

Example of logged data:
```
Musk Effect:
bitcoin (Crypto ID: bitcoin):
Name: bitcoin
Symbol: btc
Price: 30000
  - Tweet: Bitcoin is awesome!
  - Timestamp: 2023-07-24T12:34:56Z
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.

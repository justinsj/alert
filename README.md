# Alert
Simple code to send an alert

## Installation
```
python -m pip install -r requirements.txt
```

## Setup

1. Change the SLACK_WEBHOOK_URL in `secrets.py`. To get a slack webhook url, go to [https://api.slack.com/messaging/webhooks](https://api.slack.com/messaging/webhooks).

2. Change the DEFAULT_SLACK_CHANNEL in `secrets.py`.

3. Ensure that the alert code is executable
```
chmod +x alert
```
4. Copy the file to an easily accessible location like `~/alert`.
```
cp alert ~/alert
```

## Usage
```
~/alert hello
```

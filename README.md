# Alert
Simple code to send an alert

## Installation
```
sudo pip install setuptools-rust
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

## Setup

1. Change the SLACK_WEBHOOK_URL in `alert`. To get a slack webhook url, go to [https://api.slack.com/messaging/webhooks](https://api.slack.com/messaging/webhooks).

2. Change the DEFAULT_SLACK_CHANNEL in `alert`.

3. Ensure that the alert code is executable
```
chmod +x alert
```
4. Copy the file to an easily accessible location like `~/alert`.
```
cp alert ~/alert
```

## Usage
Default message `OK!`:
```
~/alert
```
Custom message:
```
~/alert hello
```

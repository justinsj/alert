# Alert
Simple code to send an alert

## Setup
1. Clone the repository
```
git clone https://github.com/justinsj/alert-git
```
2. Install the requirements
```
sudo pip install setuptools-rust
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```
3. Set up your Slack webhook URL. To do this, check out [https://api.slack.com/messaging/webhooks](https://api.slack.com/messaging/webhooks).

4. Change the SLACK_WEBHOOK_URL and DEFAULT_SLACK_CHANNEL in `alert`.

5. Ensure that the alert code is executable
```
chmod +x alert
```
6. Copy the file to an easily accessible location like `~/alert`.
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

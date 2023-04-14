# Alert
Simple code to send an alert

## Setup
1. Clone the repository
```
cd ~
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

### Error handling
If you get the error:
```
Traceback (most recent call last):
  File "/home/ubuntu/alert", line 2, in <module>
    from knockknock import slack_sender
ModuleNotFoundError: No module named 'knockknock'
```
Try:
```
which python
```
Then replace the shebang `#!/usr/local/python` in the first line of the `~/alert` file with the output.
For example:
```
#!/home/ubuntu/miniconda3/bin/python
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

## Cleanup
Once the main ~/alert file is there, you can delete this repository:
```
rm -rf ~/alert-git
```

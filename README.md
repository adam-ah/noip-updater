# noip-updater

Update noip address from the command line - rest + python

Simply supstitute your details into the script and schedule to run it. 

By default it will update noip to the address you are calling from, but you can pass in another IP as well.

```
username = "your@email.com"
password_base64 = "your.base64.encoded.password="
domain = "mydomain.noip.com"
target_ip = "" # If it's different from your current public IP
```

Use any tools to encode your password into base 64, such as https://codebeautify.org/base64-encode

Then shedule it with crontab to run every 30 minutes

```
*/30 * * * * ~/noip/update >> ~/noip/update.log
```

---
description: This page will help you getting started with the StreamElements API.
---

# Getting Started

## Get your Channel ID and Authentication Token

Simply visit the [Stream Elements Dashboard's Channel Page](https://streamelements.com/dashboard/account/channels).\
You will need to copy down 2 strings, the Account ID (aka Channel ID) and the JWT Token.
To view the JWT Token click the toggle button labeled "Show secrets".

You should have some values like these:
```
Account ID: AAABBBCCC111222333DDD123
JWT Token: AAABBBCCC111222333DDD123AAABBBCCC111.AAABBBCCC111222333DDD123AAABBBCCC111222333DDD123AAABBBCCC111222333DDD123AAABBBCCC111222333DDD123AAABBBCCC111222333DDD123AAABBBCCC111222333DDD123AAABBBCCC111222333DDD123AAABBBCCC111222333DDD123AAABBBCCC111222333DDD123AAABBBCCC111222333DDD123AAABBBCCC1112223.AAABBBCCC111-AAABBBCCC111222333DDD12-AAABBB
```

## Make your first API Call

The following Python 3 script (that uses the requests package) shows how send a simple authenticated request to the API endpoint `/kappa/v2/channels/:CHANNEL`, fill in the values you copied previously into the script and give it a shot:

```python
import requests

# Found at `https://streamelements.com/dashboard/account/channels` as `Account ID` 24 letters:
CHANNEL = "<YOUR_CHANNEL_ID>"
# Found at `https://streamelements.com/dashboard/account/channels` as `JWT Token` ~337 letters:
TOKEN = "<YOUR_JWT_TOKEN"
HEADERS = {
    "Authorization": "Bearer {}".format(TOKEN),
}

url = "https://api.streamelements.com/kappa/v2/channels/{}".format(CHANNEL)
resp = requests.get(url, headers=HEADERS)
print(resp.content)

```




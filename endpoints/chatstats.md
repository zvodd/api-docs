# Chatstats

{% api-method method="get" host="https://api.streamelements.com" path="/kappa/v2/chatstats/?limit=5" %}
{% api-method-summary %}
Get top channels
{% endapi-method-summary %}

{% api-method-description %}
Get top chatstats channels
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="limit" type="integer" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="offset" type="integer" required=false %}

{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
[
    {
        "channel": "forsen",
        "messages": 93050644
    },
    {
        "channel": "sodapoppin",
        "messages": 50531988
    },
    {
        "channel": "twitchplayspokemon",
        "messages": 49843045
    },
    {
        "channel": "loltyler1",
        "messages": 43361492
    },
    {
        "channel": "reckful",
        "messages": 42596551
    }
]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.streamelements.com" path="/kappa/v2/chatstats/search" %}
{% api-method-summary %}
Search for channel
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="channel" type="string" required=true %}
Channel username to search for
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
[
    "xd00bsd",
    "xd1324bx",
    "xd13_",
    "xd191",
    "xd1as",
    "xd21395845",
    "xd24256121",
    "xd303",
    "xd3bit",
    "xd3ivid",
    "xd3mon3x",
    "xd3rn0",
    "xd3stroyah",
    "xd428777",
    "xd4475458",
    "xd4kfull",
    "xd4nkbuds420x",
    "xd4rk_galaxy",
    "xd4vv1d",
    "xd6912369xd",
    "xd7eem_",
    "xd9955613",
    "xd_alto",
    "xd_feeder",
    "xd_gaming_05",
    "xd_klykpl_xd",
    "xd_line",
    "xd_monky_xd",
    "xd_ozzie",
    "xd_regen",
    "xd_shadow323xd",
    "xd_sxc",
    "xdaawn",
    "xdabeat",
    "xdabxqueenx420x",
    "xdac0",
    "xdaddylonglegs",
    "xdadepsak",
    "xdaesae756",
    "xdaethstar",
    "xdaeyeonx",
    "xdafox",
    "xdaft_clueless",
    "xdagarwynn",
    "xdahveedx",
    "xdaisygaming",
    "xdakurlz",
    "xdalederiate",
    "xdaltx",
    "xdamineh"
]
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.streamelements.com" path="/kappa/v2/chatstats/:username" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="username" type="string" required=true %}
The channels twitch username
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "username": "stylerdev",
  "emotes": {
    "bttvChannelEmotes": {
      "KKaper": {
        "name": "KKaper",
        "_id": "566d3352fb7103f332d79dbe",
        "type": "bttv",
        "width": 28,
        "height": 28,
        "gif": true
      },
      "KKorner": {
        "name": "KKorner",
        "_id": "5674bb22bf317838643c7de9",
        "type": "bttv",
        "width": 28,
        "height": 28,
        "gif": true
      },
      "gachiGASM": {
        "name": "gachiGASM",
        "_id": "55999813f0db38ef6c7c663e",
        "type": "bttv",
        "width": 28,
        "height": 28,
        "gif": false
      },
      "pajaDank": {
        "name": "pajaDank",
        "_id": "568d840001ea6722348ab018",
        "type": "bttv",
        "width": 28,
        "height": 28,
        "gif": false
      },
      "pajaSWA": {
        "name": "pajaSWA",
        "_id": "5738dc6ad7a0b60d147270a0",
        "type": "bttv",
        "width": 28,
        "height": 28,
        "gif": true
      }
    },
    "bttvGlobalEmotes": {}
  },
  "lastMessage": "2018-05-09T15:13:38.792784692Z",
  "settings": {
    "ignoredChatters": {}
  }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}


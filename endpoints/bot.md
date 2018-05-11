# Bot

{% api-method method="get" host="https://api.streamelements.com" path="/kappa/v2/bot/:channel" %}
{% api-method-summary %}
Get bot
{% endapi-method-summary %}

{% api-method-description %}
Retrieve basic information about the bot status.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="channel" type="string" required=true %}
Channel Id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="authorization" type="string" required=true %}
JWT Bearer token
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
    "bot": {
        "enabled": true,
        "name": "streamelements",
        "joined": true,
        "muted": false,
        "mod": true,
        "allowCustomName": true,
        "logs": [],
        "channel": "577c0455f9a31ea72a36b2b3"
    }
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.streamelements.com" path="/kappa/v2/bot/:channel/part" %}
{% api-method-summary %}
Join the bot
{% endapi-method-summary %}

{% api-method-description %}
Make the bot join your channel.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="channel" type="string" required=true %}
Channel id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="authorization" type="string" required=true %}
JWT Bearer token
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.streamelements.com" path="/kappa/v2/bot/:channel/join" %}
{% api-method-summary %}
Join the bot
{% endapi-method-summary %}

{% api-method-description %}
Make the bot part your channel
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="channel" type="string" required=true %}
Channel id
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="authorization" type="string" required=true %}
Channel id
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}


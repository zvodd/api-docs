# Bot

{% api-method method="get" host="https://api.streamelements.com" path="/kappa/v2/activities/:channel" %}
{% api-method-summary %}
Get activities
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="channel" type="string" required=true %}
The channels ID
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authorization" type="string" required=true %}
Authentication token to track down who is emptying our stocks.
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
[
  {
    "_id": "59e25ed28f25ce00010a0212",
    "channel": "59e10187207b2900014d14d9",
    "type": "tip",
    "data": {
      "tipId": "59e25ed28f25ce00010a0211",
      "username": "xd",
      "amount": 21,
      "currency": "USD",
      "message": "NaM"
    },
    "createdAt": "2017-10-14T19:00:34.324Z",
    "provider": "twitch"
  }
]
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "message": "Ain't no cake like that."
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}




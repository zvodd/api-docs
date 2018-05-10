# Activities

{% api-method method="get" host="https://api.streamelements.com" path="/kappa/v2/activities/:channel" %}
{% api-method-summary %}
Get activities for a channel
{% endapi-method-summary %}

{% api-method-description %}
This endpoint retrieves the activities for a channel.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="channel" type="string" required=true %}
channel ID
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="authorization" required=true %}
Authorization bearer token
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="types" type="string" %}
**Allowed types:  
- **follow  
- tip  
- host  
- raid  
- subscriber  
- cheer  
- redemption  
- sponsor  
- superchat
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Activities successfully retrieved.
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

{% api-method-response-example httpCode=302 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=403 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "statusCode": 404,
    "error": "Not Found"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.streamelements.com" path="/kappa/v2/activities/:channel/:activityId" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}
This endpoint retrieves a single activity for a channel.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="activityId" type="string" required=true %}
Activity ID
{% endapi-method-parameter %}

{% api-method-parameter name="channel" type="string" required=true %}
channel ID
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="authorization" required=true %}
Authorization bearer token
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
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
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=400 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
    "statusCode": 400,
    "error": "Bad Request",
    "message": "child \"channel\" fails because [\"channel\" with value \"57209398234\" fails to match the required pattern: /^[0-9a-fA-F]{24}$/]",
    "details": [
        {
            "path": [
            "channel"
            ],
            "message": "\"channel\" with value \"57209398234\" fails to match the required pattern: /^[0-9a-fA-F]{24}$/"
        }
    ]
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
    "statusCode": 401,
    "error": "Unauthorized",
    "message": "No authorization token was found"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=403 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
    "statusCode": 404,
    "error": "Not Found"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}


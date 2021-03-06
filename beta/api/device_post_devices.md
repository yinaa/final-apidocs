# Create Device

Use this API to create a new Device.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /deviceConfiguration

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer <token>. Required. |

### Request body
In the request body, supply a JSON representation of [Device](../resources/device.md) object.


### Response
If successful, this method returns `201, Created` response code and [Device](../resources/device.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_device_from_devices"
}-->
```http
POST https://graph.microsoft.com/beta/devices
Content-type: application/json
Content-length: 364

{
  "device": {
    "accountEnabled": true,
    "alternativeSecurityIds": [
      {
        "type": 99,
        "identityProvider": "identityProvider-value",
        "key": "key-value"
      }
    ],
    "approximateLastSignInDateTime": "datetime-value",
    "deviceId": "deviceId-value",
    "deviceMetadata": "deviceMetadata-value",
    "deviceVersion": 99
  }
}
```
In the request body, supply a JSON representation of [device](../resources/device.md) object.
##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device"
} -->
```http
Content-type: application/json
Content-length: 364

{
  "device": {
    "accountEnabled": true,
    "alternativeSecurityIds": [
      {
        "type": 99,
        "identityProvider": "identityProvider-value",
        "key": "key-value"
      }
    ],
    "approximateLastSignInDateTime": "datetime-value",
    "deviceId": "deviceId-value",
    "deviceMetadata": "deviceMetadata-value",
    "deviceVersion": 99
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create Device",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
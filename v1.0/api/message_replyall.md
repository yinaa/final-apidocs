# message: replyAll


### Prerequisites
One of the following **scopes** is required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /users/<id>/messages/<id>/Microsoft.Graph.replyAll
POST /drive/root/createdByUser/messages/<id>/Microsoft.Graph.replyAll
POST /drive/root/lastModifiedByUser/messages/<id>/Microsoft.Graph.replyAll

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| Authorization  | string  | Bearer %token% |

### Request body
In the request body, provide a JSON object with the following parameters.

| Parameter	   | Type	|Description|
|:---------------|:--------|:----------|
|comment|String||

### Response
If successful, this method returns `200, OK` response code. It does not return anything in the response body.

### Example
Here is an example of how to call this API.
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/<id>/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### Response
Here is an example of the response. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
#### **GET** _/roles_
``` json
# HTTP/1.1 200 OK
# Content-Type: application/vnd.api+json

{
  "data": [
    {
      "type": "roles",
      "id": "1",
      "attributes": {
	"title": "Adjunct Philosopher",
	"organization": "Acme Corp."
      }
    },
    {
      "type": "roles",
      "id": "2",
      "attributes": {
	"title": "Chief Muffin Warden",
	"organization": "Amalgamated Industries"
      }
    }
  ]
}
```


#### **GET** _/roles/1_
``` json
# HTTP/1.1 200 OK
# Content-Type: application/vnd.api+json

{
  "data": {
      "type": "roles",
      "id": "1",
      "attributes": {
	"title": "Adjunct Philosopher",
	"organization": "Acme Corp.",
	"start_date": "2000-02-01 00:00:00-5:00",
	"end_date": "203-05-01 00:00:00-5:00",
	"contact_email": "hufflewump@acmecorp.com"
      }
    }
}
```


#### Errors
``` json
HTTP/1.1 404 Not Found
Content-Type: application/vnd.api+json

{
  "errors": [
    {
      "status": "404",
      "source": {
        "pointer": "/roles/44"
      },
      "detail": "Resource not found."
    }
  ]
}
```

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
	"organization": "Acme Corp."
      }
    }
}
```

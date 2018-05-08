# JSON Server

> Quickly bring up a JSON server to play with

## Links

* https://www.codementor.io/ayushgupta/how-to-use-json-server-to-create-mock-apis-0-lci958ear

## Usage Examples

```
json-server --watch db.json
```

```
curl -X GET 'http://localhost:3000/notes'
curl -X POST -H "Content-Type: application/json" -d '{
  "id": 104,
  "body": "lala"
}' 'http://localhost:3000/notes'
curl -X GET 'http://localhost:3000/notes/104'
curl -X PUT -H 'Content-Type: application/json' -d '{"body":"tra lala"}' 'http://localhost:3000/notes/104'
curl -X DELETE -H 'Content-Type: application/json' 'http://localhost:3000/notes/104'

# Search
curl -X GET 'http://localhost:3000/notes?q=foo'

# Filters
curl -X GET 'http://localhost:3000/notes?body=flap+jacks+here'
curl -X GET 'http://localhost:3000/notes?body=flap+jacks+here&title=flap+jacks+here'
```
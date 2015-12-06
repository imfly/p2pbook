# Dapp Api

dapp.id = 9684768972206188859 

#### Api root '/'

```
// route '/' 

=> http://localhost:7040/api/dapps/9684768972206188859/api/
=> {"response":{"test":"Hello, world!"},"success":true}
```

#### default

In the `routes.json`

#### Test

curl -XPUT -H "Content-type: application/json" -d '{
"recipientId": "58191895912485C",
"message": "Hello, world!",
"secret": "test"
}' 'http://localhost:7040/api/dapps/9684768972206188859/api/messages/add'

curl -XGET 'http://localhost:7040/api/dapps/9684768972206188859/api/messages/list?recipientId=58191895912485C'

18298233975495868793C
curl -XPUT -H "Content-type: application/json" -d '{
"recipientId": "18298233975495868793C",
"message": "Hello, world!",
"secret": "test"
}' 'http://localhost:7040/api/dapps/11700699929086527232/api/messages/add'

curl -XGET 'http://localhost:7040/api/dapps/11700699929086527232/api/messages/list?recipientId=18298233975495868793C'

18298233975495868793C

/dapps/api/11700699929086527232/api/messages/list
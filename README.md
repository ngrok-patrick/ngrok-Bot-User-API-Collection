# ngrok Bot User API Collection

This is a Sample Postman Collection for using the ngrok Bot User API

This is a simple Postman Collection to get folks started using the new ngrok Bot Users API<br/>
[ngrok Bot User Collection](https://github.com/ngrok-patrick/ngrok-Bot-User-API-Collection/blob/main/ngrok%20Bot%20User%20API%20Collection.json)

Of if you like, you can just Paste the Curl Requests into Postman 

### Create Bot User
`curl --location 'https://api.ngrok.com/bot_users' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer PUT_YOUR_NGROK_API_KEY_HERE' \
--data '{
    "name":"new bot user from API",
    "active": true
}'`

### Fetch Bot User
`curl --location 'https://api.ngrok.com/bot_users/bot_2fW4JZ4hIr5NaXOUh1Je7SIUahi' \
--header 'Authorization: Bearer PUT_YOUR_NGROK_API_KEY_HERE'`

### Inactivate Bot User
`curl --location --request PATCH 'https://api.ngrok.com/bot_users/bot_2fW4JZ4hIr5NaXOUh1Je7SIUahi' \
--header 'Content-Type: application/json' \
--header 'Authorization: Bearer PUT_YOUR_NGROK_API_KEY_HERE' \
--data '{
    "active": false
}'`

### Delete Bot User
`curl --location --request DELETE 'https://api.ngrok.com/bot_users/bot_2fW4JZ4hIr5NaXOUh1Je7SIUahi' \
--header 'Authorization: Bearer PUT_YOUR_NGROK_API_KEY_HERE'`

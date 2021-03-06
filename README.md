# Waiter Tools Services

WaiterTools is a NodeJs API to get information from a restaurant created in WApp using the associated user and password.


## Installation & Run

Use the package manager NPM to install WaierTools.
```bash
npm install
```
Make sure you have the following variables properly configured in your local machine:
```bash
$API_URL
```
And finally, use the custom script to run the server.
```bash
npm start
```

# REST API
There are different endpoints to process and get data: 

## Authentication
### Request
`POST /api/v1/authentication`

    {
        "authenticationType": "Basic ",
        "authenticationCredentials": "$HASH"
    }

### Response
    HTTP/1.1 200 OK
    Date: Thu, 24 Feb 2011 12:36:32 GMT
    Status: 200 OK
    Connection: close
    Content-Type: application/json
    Content-Length: 168

    {"email":"123@waitertools.com","firstName":"Sal","lastName":"Lome",
    "restaurantId":"cc3d4fa20e2","restaurantName":"Areperia","waiterioToken":"715cb5715cb5"
    }

## Todo
- [ ] Add todo tasks
- [ ] Check helmet dependency

## License
[MIT](https://choosealicense.com/licenses/mit/)
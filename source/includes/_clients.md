# Clients

## Get All Clients

```shell
curl "https://tloger-esq.herokuapp.com/api/clients"
```

> The above command returns JSON structured like this:

```json
{  
  "status":"SUCCESS",
  "data":[  
    {  
      "id":1,
      "name":"client one",
      "createdAt":"2015-02-24T02:12:09.000Z",
      "updatedAt":"2015-02-24T16:13:51.000Z",
      "projects":[  
        {  
          "id":271,
          "name":"asdas",
          "createdAt":"2015-02-24T16:27:49.000Z",
          "updatedAt":"2015-02-24T16:27:49.000Z",
          "clientId":1
        }
      ]
    }
  ]
}
```

This endpoint retrieves list of all clients.

### HTTP Request

`GET https://tloger-esq.herokuapp.com/api/clients`


## Get Single Client

```shell
curl "https://tloger-esq.herokuapp.com/api/clients/1"
```

> The above command returns JSON structured like this:

```json
{  
  "status":"SUCCESS",
  "data":{  
    "id":1,
    "name":"client one",
    "createdAt":"2015-02-24T02:12:09.000Z",
    "updatedAt":"2015-02-24T16:13:51.000Z",
    "projects":[  
      {  
        "id":271,
        "name":"asdas",
        "createdAt":"2015-02-24T16:27:49.000Z",
        "updatedAt":"2015-02-24T16:27:49.000Z",
        "clientId":1
      }
    ]
  }
}
```

This endpoint retrieves a single client based on the id passed as parameter.

### HTTP Request

`GET https://tloger-esq.herokuapp.com/api/clients/1`


## Save Client

```shell
curl "https://tloger-esq.herokuapp.com/api/clients"
```

This endpoint is used to save the client.

### HTTP Request

`POST https://tloger-esq.herokuapp.com/api/clients`

## Delete Client

```shell
curl "https://tloger-esq.herokuapp.com/api/clients/1"
```


### HTTP Request
`DELETE https://tloger-esq.herokuapp.com/api/clients/1`


### URL Parameters
Parameter | Description
--------- | -----------
ID | The ID of the client to delete

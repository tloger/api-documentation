# Projects

## Get All Projects

```shell
curl "https://tloger-esq.herokuapp.com/api/projects"
```

> The above command returns JSON structured like this:

```json
{  
  "status":"SUCCESS",
  "data":[  
    {  
      "id":261,
      "name":"asda",
      "createdAt":"2015-02-24T16:26:25.000Z",
      "updatedAt":"2015-02-24T16:26:25.000Z",
      "client":{  
        "id":11,
        "name":"client two",
        "createdAt":"2015-02-24T02:12:17.000Z",
        "updatedAt":"2015-02-24T16:13:42.000Z"
      }
    }
  ]
}
```

This endpoint retrieves list of all projects.

### HTTP Request

`GET https://tloger-esq.herokuapp.com/api/projects`


## Get Single Project

```shell
curl "https://tloger-esq.herokuapp.com/api/projects/1"
```

> The above command returns JSON structured like this:

```json
{
  "status":"SUCCESS",
  "data":{  
    "id":261,
    "name":"asda",
    "createdAt":"2015-02-24T16:26:25.000Z",
    "updatedAt":"2015-02-24T16:26:25.000Z",
    "clientId":11,
    "tasks":[  
      {  
        "id":91,
        "name":"asdaxaSASDADA",
        "createdAt":"2015-02-24T20:10:57.000Z",
        "updatedAt":"2015-02-24T20:11:14.000Z",
        "projectId":261
      }
    ]
  }
}
```

This endpoint retrieves a single project based on the id passed as parameter.

### HTTP Request

`GET https://tloger-esq.herokuapp.com/api/projects/1`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the project to retrieve
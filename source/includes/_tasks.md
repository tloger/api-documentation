# Tasks

## Get All Tasks

```shell
curl "https://tloger-esq.herokuapp.com/api/tasks"
```

> The above command returns JSON structured like this:

```json
{  
  "status":"SUCCESS",
  "data":[  
    {  
      "id":91,
      "name":"asdaxaSASDADA",
      "createdAt":"2015-02-24T20:10:57.000Z",
      "updatedAt":"2015-02-24T20:11:14.000Z",
      "project":{  
        "id":261,
        "name":"asda",
        "createdAt":"2015-02-24T16:26:25.000Z",
        "updatedAt":"2015-02-24T16:26:25.000Z",
        "clientId":11
      }
    }
  ]
}
```

This endpoint retrieves list of all tasks.

### HTTP Request

`GET https://tloger-esq.herokuapp.com/api/tasks`


## Get Single Task

```shell
curl "https://tloger-esq.herokuapp.com/api/tasks/1"
```

> The above command returns JSON structured like this:

```json
{  
  "status":"SUCCESS",
  "data":{  
    "id":91,
    "name":"asdaxaSASDADA",
    "createdAt":"2015-02-24T20:10:57.000Z",
    "updatedAt":"2015-02-24T20:11:14.000Z",
    "projectId":261,
    "tasklogs":[  

    ]
  }
}
```

This endpoint retrieves a single task based on the id passed as parameter.

### HTTP Request

`GET https://tloger-esq.herokuapp.com/api/tasks/1`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the task to retrieve

## Save Task

```shell
curl "https://tloger-esq.herokuapp.com/api/tasks"
```

This endpoint is used to save the task.

### HTTP Request

`POST https://tloger-esq.herokuapp.com/api/tasks`

## Delete Task

```shell
curl "https://tloger-esq.herokuapp.com/api/tasks/1"
```


### HTTP Request
`DELETE https://tloger-esq.herokuapp.com/api/tasks/1`


### URL Parameters
Parameter | Description
--------- | -----------
ID | The ID of the task to delete
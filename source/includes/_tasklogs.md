# Tasklogs

## Get All Tasklogs

```shell
curl "https://tloger-esq.herokuapp.com/api/tasklogs"
```

> The above command returns JSON structured like this:

```json
{  
  "status":"SUCCESS",
  "data":[  

  ]
}
```

This endpoint retrieves list of all tasklogs.

### HTTP Request

`GET https://tloger-esq.herokuapp.com/api/tasklogs`


## Get Single Tasklog

```shell
curl "https://tloger-esq.herokuapp.com/api/tasklogs/1"
```

> The above command returns JSON structured like this:

```json
{  
  "status":"SUCCESS",
  "data":null
}
```

This endpoint retrieves a single tasklog based on the id passed as parameter.

### HTTP Request

`GET https://tloger-esq.herokuapp.com/api/tasklogs/1`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the tasklog to retrieve

## Save TaskLogs

```shell
curl "https://tloger-esq.herokuapp.com/api/tasklogs"
```

This endpoint is used to save the tasklog.

### HTTP Request

`POST https://tloger-esq.herokuapp.com/api/tasklogs`

## Delete Tasklog

```shell
curl "https://tloger-esq.herokuapp.com/api/tasklogs/1"
```


### HTTP Request
`DELETE https://tloger-esq.herokuapp.com/api/tasklogs/1`


### URL Parameters
Parameter | Description
--------- | -----------
ID | The ID of the tasklog to delete
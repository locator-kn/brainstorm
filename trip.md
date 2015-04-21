# Trip

### Routes
####GET

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/trips   | return all trips | json object | statusCode: 404 | 
|/trips/:tripID   |  return a particular trip by id | json object | statusCode: 404 | 


####POST
|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/trips   | create new trip  | statusCode: 200 | statusCode: 404 |

####PUT
|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/trips/:tripID   | update particular trip by id  | statusCode: 200 | statusCode: 404 |

####DELETE
|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/trips/:tripID   | delete particular trip by id  | statusCode: 200 | statusCode: 404 |


### Dummy Json Results
##### Specific Trip
```
{
  "_id": "1849ef313fbc39f078084f9168000e16",
  "_rev": "4-c726329a4e810962443ce5a7a176b00c",
  "title": "my trip",
  "description": "bla bla bla",
  "city": "constance",
  "start_date": "2015-04-20T00:00:00.000Z",
  "end_date": "2015-04-23T00:00:00.000Z",
  "budget": 100,
  "locations": [],
  "pics": [],
  "category": "halli galli drecksaufest",
  "type": "trip"
}
```

##### Multiple Trips, filtered by arguments 
(unterschied: pics --> titlepic, liefert einfach das erste bild, weitere bilder kommen dann erst in einer extra view, in der die obere Anfrage verwendet wird)
```
[
    {
        "_id":"1849ef313fbc39f078084f9168000e16",
        "_rev":"4-c726329a4e810962443ce5a7a176b00c",
        "title":"my trip",
        "description":"bla bla bla",
        "city":"constance",
        "start_date":"2015-04-20T00:00:00.000Z",
        "end_date":"2015-04-23T00:00:00.000Z",
        "budget":100,
        "locations":[

        ],
        "titlePic":[

        ],
        "category":"halli galli drecksaufest",
        "type":"trip"
    },
    {
        "_id":"1849ef313fbc39f078084f9168000e16",
        "_rev":"4-c726329a4e810962443ce5a7a176b00c",
        "title":"my trip",
        "description":"bla bla bla",
        "city":"constance",
        "start_date":"2015-04-20T00:00:00.000Z",
        "end_date":"2015-04-23T00:00:00.000Z",
        "budget":100,
        "locations":[

        ],
        "titlePic":[

        ],
        "category":"halli galli drecksaufest",
        "type":"trip"
    },
    {
        "_id":"1849ef313fbc39f078084f9168000e16",
        "_rev":"4-c726329a4e810962443ce5a7a176b00c",
        "title":"my trip",
        "description":"bla bla bla",
        "city":"constance",
        "start_date":"2015-04-20T00:00:00.000Z",
        "end_date":"2015-04-23T00:00:00.000Z",
        "budget":100,
        "locations":[

        ],
        "titlePic":[

        ],
        "category":"halli galli drecksaufest",
        "type":"trip"
    },
    {
        "_id":"1849ef313fbc39f078084f9168000e16",
        "_rev":"4-c726329a4e810962443ce5a7a176b00c",
        "title":"my trip",
        "description":"bla bla bla",
        "city":"constance",
        "start_date":"2015-04-20T00:00:00.000Z",
        "end_date":"2015-04-23T00:00:00.000Z",
        "budget":100,
        "locations":[

        ],
        "titlePic":[

        ],
        "category":"halli galli drecksaufest",
        "type":"trip"
    }
]
```

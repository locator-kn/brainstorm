# Trip

### Routes
####GET

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/trips   | return all trips | json object | statusCode: 404 | 
|/trips/:tripID   |  return a particular trip by id | json object | statusCode: 404 | 
|/trips/konstanz/?budget=100&checkin=01.08.2010&checkout=02.08.2010   | search for a trip | json object with all matches | statusCode: 404 | 
/armani_braun/?budget=100&season_name=frühjahr-sommer
|/data/moods   | return all moods as array **toReview** | jason array  | statusCode: 404 | 


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
##### Specific Trip - GET /trips/:tripID
```
{
  "_id": "1849ef313fbc39f078084f9168000e16",
  "_rev": "4-c726329a4e810962443ce5a7a176b00c",
  "title": "my trip",
  "local": "42312312",
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

##### Multiple Trips, filtered by arguments - GET /trips
(whats the difference? We should provide a thumbnail in the trip overview, not an array of big size pics)
```
[
    {
        "_id":"1849ef313fbc39f078084f9168000e16",
        "_rev":"4-c726329a4e810962443ce5a7a176b00c",
        "title":"my trip",
        "local": "42312312",
        "description":"bla bla bla",
        "city":"constance",
        "start_date":"2015-04-20T00:00:00.000Z",
        "end_date":"2015-04-23T00:00:00.000Z",
        "budget":100,
        "locations":[

        ],
        "thumbnail":[

        ],
        "category":"halli galli drecksaufest",
        "type":"trip"
    },
    {
       ...
    },
    {
      ...
    },
    {
      ...
    }
]
```


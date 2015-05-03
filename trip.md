# Trip

### Routes
####GET

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/trips   | return all trips | json object | statusCode: 404 | 
|/trips/:tripID   |  return a particular trip by id | json object | statusCode: 404 | 
|/trips/search/*(see below)   | search for a trip | json object with all matches | statusCode: 404 |
*/trips/search/78467_mood1.mood2.mood3/?budget=100&checkin=2015-05-17&checkout=2015-05-19&persons=3



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

### Search

|Parameter| optional / required | info |
|---|---|---|
|city| required | /trips/**city**|
|mood| optional | /trips/**_mood1_mood2_mood3**|
|city/mood| required| /trips/**city_mood1_mood2**|
|checkin/checkout| optional | /trips/city_mood1/**?checkin=2015-05-15&checkout=2015-05-05** - if committed, use db query to get only trips between checkin and checkout|
|days|optional|/trips/city_mood1/**?days=2**|
|persons|optional|/trips/city_mood1/**?persons=3**|
|budget|optional|/trips/city_mood1/**?budget=56**|


### Dummy Json Results
##### Specific Trip - GET /trips/:tripID
```
{
  "_id": "1849ef313fbc39f078084f9168000e16",
  "_rev": "4-c726329a4e810962443ce5a7a176b00c",
  "title": "my trip",
  "local": "42312312",
  "description": "bla bla bla",
  "postcode": "78467",
  "city": "constance",
  "start_date": "2015-04-20T00:00:00.000Z",
  "end_date": "2015-04-23T00:00:00.000Z",
  "days": "2",
  "persons": "3",
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
        "postcode": "78467",
        "city":"constance",
        "start_date":"2015-04-20T00:00:00.000Z",
        "end_date":"2015-04-23T00:00:00.000Z",
        "days": "2",
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


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

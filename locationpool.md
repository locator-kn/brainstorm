# Documents

### Beschreibung
Jeder _local_ hat ein pool an seinen favorisierten location, die er "cool" findet. Eine Location Besteht aus:
 - einem Ort (Name) (o.ä.?)
 - Bilder (+ Thumbnail)
 - Geotag
 - Beschreibung 
 - URL zu Bild
 - und/oder ???

Der Locationpool eines Benutzers besteht aus einer _leichtgewichtige_ Liste aller Locations. //TODO: diskutieren.


### Routes
####GET

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/user/:userID/locations/  | returns a locationpool (list) of saved location of the user   | json object | statusCode: 404 |
|/user/[c:red][:userID]/locations/:locationsID (user id nötig??) | returns a particular saved location of the user | json object | statusCode: 404 |

####POST

|Ressource   | Description  | on Failure |
|---|---|---|---|
|/user/:userID/locations/  | adds a location into the location pool of the user   |  statusCode: 404 |

Note: Bulk add will be done if payload is array.

####PUT


|Ressource   | Description  | on Failure |
|---|---|---|---|
|/user/:userID/locations/:locationsID  | updates a location of the location pool of the user   |  statusCode: 404 |



### Dummy json results

```

```

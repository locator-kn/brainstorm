# Board

### Routes
####GET

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/boards/:postID   | return particular post with comments    | json object | statusCode: 404 | 
|/boards/posts/:postID  | returns post with postID    | json object | statusCode: 404 |
|/boards/groups/:groupID  | returns all post of particular group     | json object | statusCode: 404 |
|/boards/comments/:postID  | returns all comments of particular post     | json object | statusCode: 404 |

####POST

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/boards/posts/:groupID  | create new post  | statusCode 200 | statusCode: 404 |
|/boards/comments/:postID  | create new comment for particular post    | statusCode 200 | statusCode: 404 |

####PUT

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/boards/posts/:postID  | update post  | statusCode 200 | statusCode: 404 |
|/boards/comments/:commentID  | update comment  | statusCode 200 | statusCode: 404 |


### Dummy Json Results

####GET /boards/groups/:groupID
```
[
{
  "_id": "551bfb6b2926b18360873cbf",
  "date": "2014-04-23T18:25:43.511Z",
  "title": "hey yo",
  "author": "551bfb6bedba87b86375ad3b",
  "author_thumbnail": "data:image/jpg;base64,/9j/4QAYRXhpZgAASUkqAAgAAAAAAAAA...",
  "content": "Cillum consectetur proident sit adipisicing ut exercitation.",
  "comment_number": "0"
},
{
  "_id": "551bfb6b8f58d0577e3f4c1c",
  "date": "2013-04-23T18:25:43.511Z",
  "title": "was geht?",
  "author": "551bfb6b171cbd94abfb16f4",
  "author_thumbnail": "data:image/jpg;base64,/9j/4QAYRXhpZgAASUkqAAgAAAAAAAAAAAAAAP...",
  "content": "Ut reprehenderit ullamco ut ex laborum culpa eu.",
  "comment_number": "0"
},
{
  "_id": "551bfb6bc62cc7df95a3a3a9",
  "date": "2012-04-23T18:25:43.511Z",
  "title": "huhuhuhu",
  "author": "551bfb6b64f023b9f876cfa3",
  "author_thumbnail": "data:image/jpg;base64,/9j/4QAYRXhpZgAASUkqAAgAAAAAAAAAAAAAA...",
  "content": "Ut occaecat sit aliquip id quis magna irure dolore sint excepteur.",
  "comment_number": "0"
}
]

```


####GET /boards/:postID
```
{
  "_id": "551bfb6b2926b18360873cbf",
  "date": "2014-04-23T18:25:43.511Z",
  "title": "BSYS-Nachhilfe",
  "author": "551bfb6bedba87b86375ad3b",
  "author_thumbnail": "data:image/jpg;base64,/9j/4QAYRXhpZgAASUkqAAgAAAAAAAAAAAAAAP",
  "content": "Kann mir einer BSYS-Nachhilfe geben?",
  "comments_length": "2",
  "comments": [
      {
          "_id": "551bfb6b2926b18360883cbf",
          "date": "2015-04-23T18:25:43.511Z",
          "author": "551bfb6bedba87b87375ad3b",
          "author_thumbnail": "data:image/jpg;base64,/9j/4QAYRXhpZgAASUkqAAgAAAAAAAAAAAAAAP",
    "content": "Sie müssen sich besser organisieren!",
    "comments_length": "1"
},
{
    "_id": "551bfb6b2926b18360823cbf",
    "date": "2016-04-23T18:25:43.511Z",
    "author": "551bfb6bedba87b56375ad3b",
    "author_thumbnail": "data:image/jpg;base64,/9j/4QAYRXhpZgAASUkqAAgAAAAAAAAAAAAAAP",
            "content": "Heute ist Spritwoch->keine Zeit",
            "comments_length": "1"
        }
    ]
}
```


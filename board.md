# Board

### Routes
####GET

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/boards/:postID   | return particular post with comments    | json object | statusCode: 404 | 
|/boards/posts/:postID  | returns post with postID    | json object | statusCode: 404 |
|/boards/groups/:groupID  | returns all post of particular group     | json object | statusCode: 404 |
|/boards/posts/:postID/comments  | returns all comments of particular post     | json object | statusCode: 404 |

####POST

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/boards/posts  | create new post  | statusCode 200 | statusCode: 404 |
|/boards/posts/:postID/comments  | create new comment for particular post    | statusCode 200 | statusCode: 404 |

####PUT

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/boards/posts/:postID  | update post  | statusCode 200 | statusCode: 404 |
|/boards/comments/:commentID  | update comment  | statusCode 200 | statusCode: 404 |


### Dummy Json Results

#### Post

```
{
  "_id": "1111111111111111122",
  "date": "2014-04-23T18:25:43.511Z",
  "title": "hey yo",
  "author": "551bfb6bedba87b86375ad3b",
  "author_thumbnail": "data:image/jpg;base64,/9j/4QAYRXhpZgAASUkqAAgAAAAAAAAA...",
  "content": "Cillum consectetur proident sit adipisicing ut exercitation.",
  "comment_count": "0",
  "group": "123456",
  "type": "post"
}

```

#### Comment
```
{
  "_id": "551bfb6b2926b18360873cbf",
  "post_id": "1111111111111111122",
  "date": "2014-04-23T18:25:43.511Z",
  "author": "551bfb6bedba87b86375ad3b",
  "author_thumbnail": "data:image/jpg;base64,/9j/4QAYRXhpZgAASUkqAAgAAAAAAAAA...",
  "content": "Cillum consectetur proident sit adipisicing ut exercitation.",
  "type": "comment"
}

```

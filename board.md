# Board

### Routes
####GET

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/groups/:groupID/boards   | return a list of boards with boards information    | json object | statusCode: 404 | 
|/groups/:groupID/boards/:boardID  | returns a particular board    | json object | statusCode: 404 |
|/groups/:groupID/boards/:boardID/posts  | returns all posts with comments    | json object | statusCode: 404 |
|/groups/:groupID/boards/:boardID/posts/:postID  | return a particular post with comments     | json object | statusCode: 404 |
|/groups/:groupID/boards/:boardID/posts/:postID/comments  | return all comments   | json object | statusCode: 404 |
|/groups/:groupID/boards/:boardID/posts/:postID/comments/:commentID  | return a particular comment   | json object | statusCode: 404 |

####POST

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/groups/:groupID/boards   | create new board    | statusCode: 200 | statusCode: 404 | 
|/groups/:groupID/boards/:boardID/posts  | create new post    | statusCode: 200 | statusCode: 404 |
|/groups/:groupID/boards/:boardID/posts/:postID/comments  | create new comment   | statusCode: 200 | statusCode: 404 |

####PUT

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/groups/:groupID/boards/:boardID  | update board information    | statusCode: 200 | statusCode: 404 |
|/groups/:groupID/boards/:boardID/posts/:postID  | update post information     | statusCode: 200 | statusCode: 404 |
|/groups/:groupID/boards/:boardID/posts/:postID/comments/:commentID  | update comment infromation   | statusCode: 200 | statusCode: 404 |

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

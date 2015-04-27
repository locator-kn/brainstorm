### Routes
####GET

|Ressource   | Description  |  on Success | on Failure |
|---|---|---|---|
|/data/cities           | returns all available cities  | json object | statusCode: 404 |
|/data/moods | returns all available moods  | json object | statusCode: 404 | 
|/data/acc           | returns all available accomodations   | json object | statusCode: 404 |

### Dummy json results

#### cities
```
[
    {
        "_id": "551bd8d98fe8ee54fe79fbe0",
        "name": "Konstanz",
        "plz": 78764,
        "type": "city"
    },
    {
        "_id": "551bd8d96ac6271311173b03",
        "name": "Berlin",
        "plz": 13545,
        "type": "city"
    },
    {
        "_id": "551bd8d9c528474af52dbd7e",
        "name": "Hamburg",
        "plz": 24567,
        "type": "city"
    }
]
```

#### accomodations
```
[
    {
        "_id": "1",
        "name": "couch",
        "type": "acc"
    },
    {
        "_id": "2",
        "name": "room",
        "type": "acc"
    },
    {
        "_id": "3",
        "name": "holiday_flat",
        "type": "acc"
    }
]
```

#### moods
```
[
    {
        _id: '1',
        title: 'Family Fun',
        icon: '',
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
    },
    {
        _id: '2',
        title: 'Girls on Tour',
        icon: '',
        image: '',
        description: '',
        excludes: ['4', '5'],
        "type": "mood"
    },
    {
        _id: '3',
        title: 'Buddytrip',
        icon: '',
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
    },
    {
        _id: '4',
        title: 'Singles unter sich',
        icon: '',
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
    },
    {
        _id: '5',
        title: 'Sturm der Liebe',
        icon: '',
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
    },
    {
        _id: '6',
        title: 'Halligalli Drecksaufest',
        icon: '',
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
    },
    {
        _id: '7',
        title: 'Muskelkater',
        icon: '',
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
    },
    {
        _id: '8',
        title: 'Leckermäulchen',
        icon: '',,
        
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
    },
    {
        _id: '9',
        title: 'Grüner gehts nicht',
        icon: '',
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
    },
    {
        _id: '10',
        title: 'Entspannung pur',
        icon: '',
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
        
    },
    {
        _id: '11',
        title: 'Kultur und Sightseeing',
        icon: '',
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
    },
    {
        _id: '12',
        title: 'Haste nicht gesehn',
        icon: '',
        image: '',
        description: '',
        excludes: [],
        "type": "mood"
    }
]
```

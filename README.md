# format-api

Is a Search tool for accessing formats images, via api.

- Host : http://search.haystack.im

## POST - /api/v1/format
###Headers:
Content-Type: Application/JSON

###Example Request:

```js
{
    //Array of words
    "term": ["russia"],
    //Sort By
    "sorting": "rating",
    //Offset
    "offset": 0,
    //Limit number of results
    "limit": 60
}
```

###Example Responds:
````
{
  "results_total": 1,
  "results": [
    {
      "org": "format",
      "collection": "format",
      "image_id": "format_54383176",
      "key": "format_54383176",
      "id": "54383176",
      "keywords": [
        "underwater",
        "water",
        "sea",
        "fish",
        "ocean",
        "coral",
        "travel",
        "reef",
        "invertebrate",
        "nobody",
        "diving",
        "outdoors",
        "shallow",
        "swimming",
        "lagoon",
        "seascape",
        "color",
        "scuba",
        "snorkeling",
        "nature"
      ],
      "width": 1000,
      "height": 1000,
      "orientation": "Horizontal",
      "rating": 0.52558506
    }
  ]
}

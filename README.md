# Format-API

Is a Search tool for accessing Format's images, via api powered by Haystack.im.

- Host : http://search.haystack.im

## POST - /api/v1/format
###Headers:
Content-Type: Application/JSON

###Example Request:

```js
{
    //Array of words
    "term": ["water"],
    //Sort By
    "sorting": "rating",
    //Offset
    "offset": 0,
    //Limit number of results
    "limit": 60
}
```
```bash
curl -X POST -H "Content-Type: application/json" -H "Authorization: Basic bHNxOmNiMmNhZTNlNjMxZTYwZDA5MThhZjQ3ODk1NWY5MGM5" -H "Cache-Control: no-cache" -H "Postman-Token: 54e272b3-5244-10c6-6fb6-c8d18e89ec1d" -d '{
   "term": ["girl"],
   "sorting": "rating",
   "offset": 0,
   "limit": 60
}' 'http://search.haystack.im/api/v1/format'
```


###Example Responds:
````
{
  "results_total": 3,
  "results": [
    {
      "org": "format",
      "collection": "format",
      "image_id": "format_9984101",
      "key": "format_9984101",
      "id": "9984101",
      "url": "http://www.nirrimi.com",
      "headline": "b",
      "keywords": [
        "travel",
        "outdoors",
        "sky",
        "water",
        "women",
        "sunshine",
        "architecture",
        "sunset",
        "people",
        "coast",
        "leisure",
        "nobody",
        "relaxation",
        "summer",
        "city",
        "adult",
        "beach",
        "togetherness",
        "sea",
        "men"
      ],
      "thumb": "https://s3.amazonaws.com/hay-format/9984101.jpg",
      "src": "http://a2.format-assets.com/image/private/s--vnaBsmBp--/a_auto,fl_keep_iptc.progressive,q_95/25390-6798121-2b1",
      "width": "1500",
      "height": "1014",
      "orientation": "Horizontal",
      "rating": 0.6822541,
      "creator_industry": "Photography - Portrait",
      "creator_description": "Young photographer, writer & mama living all over the world and sharing goodness.",
      "creator_city": "Melton",
      "creator_region": "07",
      "creator_country": "Australia",
      "creator_site_domain": "http://www.nirrimi.com"
    },
    {
      "org": "format",
      "collection": "format",
      "image_id": "format_9984191",
      "key": "format_9984191",
      "id": "9984191",
      "url": "http://www.nirrimi.com",
      "headline": "a",
      "keywords": [
        "beach",
        "coast",
        "water",
        "sea",
        "travel",
        "ocean",
        "sand",
        "leisure",
        "barefoot",
        "solitude",
        "girl",
        "love",
        "outdoors",
        "child",
        "fun",
        "recreation",
        "carefree",
        "romance",
        "relaxation",
        "vacation"
      ],
      "thumb": "https://s3.amazonaws.com/hay-format/9984191.jpg",
      "src": "http://a4.format-assets.com/image/private/s--Ssk9nTc3--/a_auto,fl_keep_iptc.progressive,q_95/25390-6798198-3a3",
      "width": "1500",
      "height": "2234",
      "orientation": "Vertical",
      "rating": 0.68061507,
      "creator_industry": "Photography - Portrait",
      "creator_description": "Young photographer, writer & mama living all over the world and sharing goodness.",
      "creator_city": "Melton",
      "creator_region": "07",
      "creator_country": "Australia",
      "creator_site_domain": "http://www.nirrimi.com"
    },
    {
      "org": "format",
      "collection": "format",
      "image_id": "format_9984200",
      "key": "format_9984200",
      "id": "9984200",
      "url": "http://www.nirrimi.com",
      "headline": "a",
      "keywords": [
        "beach",
        "relaxation",
        "summer",
        "sexy",
        "leisure",
        "women",
        "portrait",
        "people",
        "one",
        "adult",
        "sand",
        "vacation",
        "brunette",
        "enjoyment",
        "water",
        "nude",
        "girl",
        "tan",
        "lifestyle",
        "love"
      ],
      "thumb": "https://s3.amazonaws.com/hay-format/9984200.jpg",
      "src": "http://a2.format-assets.com/image/private/s--6Opbh5sm--/a_auto,fl_keep_iptc.progressive,q_95/25390-6798207-3a5",
      "width": "1500",
      "height": "1000",
      "orientation": "Horizontal",
      "rating": 0.6665139,
      "creator_industry": "Photography - Portrait",
      "creator_description": "Young photographer, writer & mama living all over the world and sharing goodness.",
      "creator_city": "Melton",
      "creator_region": "07",
      "creator_country": "Australia",
      "creator_site_domain": "http://www.nirrimi.com"
    }
  ]
}

# Search

    GET news_headlines/_search

### Search for data within a specific time range

    GET news_headlines/_search
    {
        "query": {
            "range": {
            "date": {
                "gte": "2015-06-20",
                "lte": "2015-09-22"
            }
            }
        }
    }

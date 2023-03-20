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

### Running a match query against multiple fields

    GET Enter_the_name_of_the_index_here/_search
    {
        "query": {
            "multi_match": {
            "query": "Enter search terms here",
            "fields": [
                "List the field you want to search over",
                "List the field you want to search over",
                "List the field you want to search over"
            ]
            }
        }
    }

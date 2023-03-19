# Precision and Recall

Increasing Recall

    GET enter_name_of_index_here/_search
    {
        "query": {
            "match": {
                "Specify the field you want to search": {
                    "query": "Enter search terms"
                }
            }
        }
    }

Increasing Precision
We can increase precision by adding an "and" operator to the query.

    GET enter_name_of_index_here/_search
    {
        "query": {
            "match": {
                "Specify the field you want to search": {
                    "query": "Enter search terms",
                    "operator": "and"
                }
            }
        }
    }

# connort45.github.io
connor trevaskiss cmtrevaskiss@my.waketech.edu
this is my school account, wake tech community college 
this repository was made to hold assigments, how many i do not yet know
## About ME:

### My Interests:
Fishing,hiking, spending time with my GF, video games. Learning about cybersecurity. My goal is to become a Threat analyst, or something along those lines.

### Websites I'd Recommend:
Virus-Total-
This Mermaid diagram shows a simple flow from the start to different sections of your README.md. You can customize it further as needed.

CUSTOMERS {
    int customer_id
    string first_name
    string last_name
    string email
    string phone_number
}

SALES {
    int sale_id
    date sale_date
    int customer_id
    float total_amount
}

INVENTORY {
    int inventory_id
    int product_id
    int stock_level
}

SALES_PRODUCTS {
    int sale_id
    int product_id
}

CUSTOMERS ||--o| SALES : makes
SALES ||--o| SALES_PRODUCTS : contains
PRODUCTS ||--o| SALES_PRODUCTS : is_sold_in
PRODUCTS ||--o| INVENTORY : tracks_stock

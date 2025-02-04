erDiagram
    PRODUCTS {
        int product_id PK
        string product_name
        string size
        string color
        float price
    }

    CUSTOMERS {
        int customer_id PK
        string first_name
        string last_name
        string email
        string phone_number
    }

    SALES {
        int sale_id PK
        date sale_date
        int customer_id FK
        float total_amount
    }

    INVENTORY {
        int inventory_id PK
        int product_id FK
        int stock_level
    }

    SALES_PRODUCTS {
        int sale_id FK
        int product_id FK
    }

    CUSTOMERS ||--o| SALES : makes
    SALES ||--o| SALES_PRODUCTS : contains
    PRODUCTS ||--o| SALES_PRODUCTS : is_sold_in
    PRODUCTS ||--o| INVENTORY : tracks_stock





Customers to sales- a customer is needed to make the sale, without the customer wanting to buy the item the sale could never exist, a customer base is always needed in order to start making sales
sales contains sales products- a sale wouldnt exist if there was not a product to sell, with a product the company knows people will want to buy the item in a sale. They will use the sale to sell the items at a higher rate.
sales sell products- a sale is like an ad detailing what product is on sale and what types of that prodcut fal under the umbrella of the sale. A sale exists to help sell an underpreforming or brand new item that needs more attention.
products are tracked in inventory- during sales the items sold must be tracked, that is then reflected in the companies inventory, without a correctly working inventory the sale will fall through. The company may oversell or undersell due to incorrect inventory information. It is vital for the inventory to be correct
All of the parts work together like a well oiled machine, a company has a product to sell, they have to make sure they have a customer base, when they have the customer base they can start making the sales, the sales are then tracked in the inventory so the company can then take that informaiton an order more or order more items like that. All of thee moving parts are just as important at the other.

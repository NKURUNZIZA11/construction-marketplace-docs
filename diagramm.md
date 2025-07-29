erDiagram
    USER {
        int user_id PK
        string first_name
        string last_name
        string email UK
        string phone_number UK
        string password_hash
        enum user_type
        datetime created_at
    }
    
    PRODUCT {
        int product_id PK
        int supplier_id FK
        string product_name
        decimal price
        int stock_quantity
    }
    
    USER ||--o{ PRODUCT : "sells"

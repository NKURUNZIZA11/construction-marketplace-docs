flowchart TD
    Start([User Visits Platform]) --> UserType{User Type?}
    
    UserType -->|New User| Register[User Registration]
    UserType -->|Existing User| Login[User Login]
    
    Register --> Verify[Email/Phone Verification]
    Login --> Dashboard{User Dashboard}
    
    Dashboard -->|Buyer| BuyerDash[Buyer Dashboard]
    Dashboard -->|Supplier| SupplierDash[Supplier Dashboard]

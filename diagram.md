system-diagrams.md
# Construction Materials Marketplace - System Diagrams

## 1. Existing System Architecture

```mermaid
graph TB
    subgraph "BUYERS (Contractors, Builders, Individuals)"
        B1[Builder/Contractor]
        B2[Private Individual]
        B3[Small Construction Company]
    end
    
    subgraph "MANUAL PROCESSES"
        MP1[Physical Store Visits]
        MP2[Phone Calls]
        MP3[WhatsApp Groups]
        MP4[Manual Price Comparison]
        MP5[Cash/Check Payments]
        MP6[Paper-based Records]
    end
    
    subgraph "SUPPLIERS"
        S1[Hardware Store A]
        S2[Building Supply Store B]
        S3[Construction Material Dealer C]
        S4[Local Distributor]
    end
    
    B1 --> MP1
    B2 --> MP2
    B3 --> MP3
    
    MP1 --> S1
    MP2 --> S3
    MP3 --> S4
    
    style B1 fill:#e1f5fe
    style S1 fill:#f3e5f5


## **PROPOSED SYSTEM:**

flowchart TD
    Start([User Visits Platform]) --> UserType{User Type?}
    
    UserType -->|New User| Register[User Registration]
    UserType -->|Existing User| Login[User Login]
    
    Register --> Verify[Email/Phone Verification]
    Login --> Dashboard{User Dashboard}
    
    Dashboard -->|Buyer| BuyerDash[Buyer Dashboard]
    Dashboard -->|Supplier| SupplierDash[Supplier Dashboard]


### **ERD:**

### **💡 Pro Tips:**
1. **Use descriptive commit messages**: "Add system flowchart diagram"
2. **Create separate files** for different diagram types
3. **Add explanations** above each diagram
4. **Update regularly** as your project evolves

### **Example Repository URL:**
After creation, you'll get a link like:
`https://github.com/yourusername/construction-marketplace-docs`

## **Quick Test:**
1. Try creating just one file first with a simple diagram
2. See how it looks when rendered
3. Then add the complete diagrams

**Would you like me to help you set this up step by step?** I can guide you through creating your first repository and adding the diagrams!

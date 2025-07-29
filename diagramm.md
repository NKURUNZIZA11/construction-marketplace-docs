
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

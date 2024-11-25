# 4DESA_MiniProjet
## Social Media Platform Developement With Azure
## Key Components of the Platform:
### Authentication & Authorization
### Content Management
### API Layer
### Database & Storage
### Scalability & Performance
### Integration with Frontend Clients

### Architecture Diagram
                     +---------------------------+
                     |     Front-End Clients     |
                     |   (Web/Mobile/3rd Party)  |
                     +---------------------------+
                              |
                              v
             +----------------------------------+
             |     Azure API Management        | 
             |   (Manage APIs, Rate Limiting)  |
             +----------------------------------+
                     |             |
       +-------------+-------------+----------------+
       |             |             |                |
+--------------+  +----------------+   +------------------------+
| Azure App    |  | Azure Functions |   | Azure Logic Apps        |
| Services     |  | (Serverless API |   | (Workflow Automation)   |
| (API Layer)  |  | Layer)          |   |                        |
+--------------+  +----------------+   +------------------------+
       |              |                  |
       v              v                  v
+----------------------------+    +-----------------------+
|   Azure Cosmos DB           |    |    Azure Blob Storage |
|   (Metadata, User Data)     |    |    (User Media Files) |
+----------------------------+    +-----------------------+
       |
       v
+----------------------------+
|   Azure Redis Cache        |
|   (Caching)                |
+----------------------------+

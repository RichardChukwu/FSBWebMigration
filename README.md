## Federal Scholarship Board Website Migration to Azure

### Project Overview
This project involves migrating the Federal Scholarship Board's website from an on-premises setup to Azure Cloud to streamline the scholarship verification and renewal process. The goal is to create a scalable, secure, and cost-effective solution that enables online submission, verification, and automated payment processes for scholarship applicants.

### Problem Statement
Every year, the Federal Scholarship Board manually verifies student documents for scholarship renewal, requiring representatives to visit various universities, resulting in significant costs and inefficiencies. The current website lacks the functionality for online document submission and automated verification.

### Solution
To address these challenges, the solution involves migrating the existing website to Azure, implementing online document submission, automating the verification process, and integrating payment systems. This solution leverages various Azure services to ensure scalability, security, and cost-efficiency.

### Architecture Diagram
![Architecture Diagram](path/to/your/architecture_diagram.png)

### Azure Services Used
1. **Azure App Services**: Hosts the web application.
2. **Azure Blob Storage**: Stores submitted documents securely.
3. **Azure SQL Database**: Manages student records and verification status.
4. **Azure Logic Apps / Azure Functions**: Automates document verification and payment processes.
5. **Azure Active Directory**: Manages authentication and authorization.
6. **Azure Application Gateway**: Provides load balancing and web application firewall capabilities.
7. **Azure Monitor**: Monitors application performance and health.

### TCO Calculation
Using the Azure TCO Calculator, the total cost of ownership for running the on-premises setup versus Azure was compared over a three-year period.

#### On-Premises Costs (Example Estimate):
- **Hardware Costs**: $20,000 (servers and storage)
- **Maintenance Costs**: $5,000 per year
- **Power and Cooling**: $2,500 per year
- **Networking Costs**: $1,000 per year
- **Operational Costs**: $10,000 per year (IT staff, security, backup)

**Total On-Premises Costs for 3 Years**: Approximately $67,500

#### Azure Costs (Example Estimate):
- **Azure App Services**: $1,800 per year
- **Azure SQL Database**: $6,000 per year
- **Azure Blob Storage**: $300 per year
- **Azure Application Gateway**: $1,500 per year
- **Azure Logic Apps / Functions**: $600 per year
- **Azure Active Directory**: $0 (assuming basic tier)

**Total Azure Costs for 3 Years**: Approximately $30,900

#### Cost Savings:
Migrating to Azure could potentially save around $36,600 over three years.

### Pricing Calculator Configuration
#### Virtual Machines:
- **Region**: West US
- **Operating system**: Windows
- **Tier**: Standard
- **Instance**: D2 v3
- **Virtual machines**: 2 x 730 Hours

#### Azure SQL Database:
- **Region**: West US
- **Type**: Single Database
- **Backup storage tier**: RA-GRS
- **Purchase model**: vCore
- **Service tier**: General Purpose
- **Compute tier**: Provisioned
- **Generation**: Gen 5
- **Instance**: 8 vCore

#### Application Gateway:
- **Region**: West US
- **Tier**: Web Application Firewall
- **Size**: Medium
- **Gateway hours**: 2 x 730 Hours
- **Data processed**: 1 TB
- **Outbound data transfer**: 5 GB

### Challenges and Solutions
1. **Manual Document Verification**:
   - **Challenge**: High cost and inefficiency due to physical verification.
   - **Solution**: Implemented Azure Blob Storage for online document submission and Azure Logic Apps for automated verification.

2. **Scalability**:
   - **Challenge**: Scaling on-premises infrastructure to handle peak loads.
   - **Solution**: Used Azure App Services and Azure Application Gateway to ensure scalability and load balancing.

3. **Cost Management**:
   - **Challenge**: High operational costs of maintaining on-premises infrastructure.
   - **Solution**: Leveraged Azure's pay-as-you-go model to reduce costs and improve cost predictability.

### How to Use This Project
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/federal-scholarship-board-migration.git
   ```

2. **Navigate to the Project Directory**:
   ```bash
   cd federal-scholarship-board-migration
   ```

3. **Review the Architecture Diagram**:
   - Open the architecture diagram to understand the solution's structure.

4. **Review the TCO Report**:
   - Examine the TCO report for a detailed cost comparison.

5. **Deploy to Azure**:
   - Follow the deployment instructions provided in the repository to set up the Azure environment.

### Conclusion
This project showcases the migration of an on-premises web application to Azure, highlighting the cost savings, scalability, and efficiency gains achieved through cloud adoption. It serves as a practical example of leveraging Azure services to solve real-world problems.

For any questions or further information, please contact [richardchukwu99@gmail.com].

Project Overview:

The Online GP Appointment Booking System is a cloud-based web application that allows patients to easily search, view, and book general practitioner (GP) appointments. The application provides real-time availability, secure user authentication, and a seamless booking experience. The entire system is built using AWS serverless services to ensure scalability, high availability, cost-efficiency, and strong security controls.

AWS Services Used and Their Purpose:
- AWS Amplify – Hosts and deploys the front-end React application and manages continuous deployment from GitHub.
- Amazon Cognito – Handles user authentication, sign-up/sign-in, MFA, and secure token management.
- Amazon API Gateway – Manages REST API endpoints and routes requests between the client and backend services.
- AWS Lambda – Executes backend logic for booking, authentication validation, and email notifications.
- Amazon DynamoDB – Stores user details, appointment records, and available time slots with built-in encryption.
- AWS WAF (Web Application Firewall) – Protects the application from malicious traffic, bot attacks, and unauthorized access attempts.
- Amazon CloudWatch – Monitors logs, performance metrics, and enables troubleshooting across the system.
- AWS CloudFormation – Deploys infrastructure using Infrastructure-as-Code templates for repeatable, consistent setups.
- AWS CodePipeline – Automates CI/CD for both front-end and back-end code updates.
- AWS IAM – Applies least-privileged access controls for secure service-level permissions.

Automation (IaC + CI/CD):

The system uses Infrastructure-as-Code (IaC) through AWS CloudFormation to automatically deploy and configure all required AWS resources, ensuring consistent and repeatable environments. Continuous Integration and Continuous Deployment (CI/CD) is implemented using AWS CodePipeline with GitHub integration. This automates front-end and back-end deployments, enabling faster updates, version control, and reliable rollouts.

My key contributions to this project included both front-end development and backend/data integration tasks:

1.	Data Sourcing & Processing
-	Searched for a suitable public healthcare dataset to support appointment and analytics features.
-	Cleaned and pre-processed the dataset by removing duplicates and invalid records. Converted the dataset from CSV to JSON format.
-	Integrated the processed data into the home page and displayed insights using graphical visualizations.

2.	Front-End Development
-	Designed and built the main home page interface using ReactJS, focusing on clean layout and user-friendly navigation.
-	Ensured smooth integration between the UI and backend APIs.

3.	Backend & Security Configuration
- Worked on fixing functional issues such as the time-slot dropdown not loading due to Lambda and API Gateway permission errors.
- Updated IAM role permissions to allow secure API Gateway invocation.
- Troubleshot Cognito MFA being blocked by WAF. Reviewed CloudWatch logs, identified Bot Control Rule as the cause, and adjusted WAF rules to restore MFA functionality.
- Assisted in validating security configurations including IAM least-privilege access and role-based permissions.

Serverless Architecture of "GP Booking System"
<img width="537" height="308" alt="Screenshot 2026-03-28 at 12 11 40 PM" src="https://github.com/user-attachments/assets/bb517256-8e73-40d1-950b-b0774e646f01" />

Waf Rules
<img width="620" height="260" alt="Screenshot 2026-03-28 at 12 12 47 PM" src="https://github.com/user-attachments/assets/5ede2935-ae35-4a1e-ac27-322dcb0147a6" />

Website SSL Report & Code Vulnerability Check
<img width="620" height="260" alt="Screenshot 2026-03-28 at 12 13 16 PM" src="https://github.com/user-attachments/assets/1d0d25b1-3ba4-4e67-b112-4012004ab786" />

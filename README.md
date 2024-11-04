OPSC POE 

Student Name/No.: Utima Emerson Neto- ST10245994

CASH MATE
The Cashmate App has been tailored to enhance users' ability to control their finances. The application encompasses features, which enable users to record their expenditures, keep track of settlements, construct monetary plans, and transfer information to an offsite database. It ensures that a user has a clear picture of their financial position and can make decisions accordingly, in order to adhere to and follow their budget.
Features
Expense Management: Track daily expenses with detailed information such as name, date, note, amount, and user ID.
Budget Planning: Set up custom budgets for various categories and track your spending against those limits.
Transaction History: Keep a detailed record of all transactions to monitor the flow of your finances.
User Synchronization: Sync data between the local SQLite database and a remote server vercel (Nodejs).and mongo atlas
Push Notifications: Stay informed with notifications about transactions, budget limits, and more.
Real-time Notifications: To broadcast messages to application using firebase cloud messaging
Login: Using SOS firebase Auth, sign email and fingerprint once an initial session is authenticated


Design

User Experience (UX):
Intuitive Interface: The design prioritizes simplicity and user-friendliness.
Cross-Platform Support: This app is compatible with both Android and iOS devices.
Offline Access: Users can log expenses without an internet connection, with data synchronizing automatically once back online.
Data Management:
SQLite Database: Utilizes local storage for quicker access and offline capability.
Remote Synchronization: A background scheduler (via Work Manager) regularly synchronizes data with the server.
Data Transformations: The app processes data into a format optimized for synchronization, ensuring efficiency and minimal data loss.
Security
Data Privacy: Users' transaction details and budgets are securely stored and transferred using encrypted channels.
Authentication: Plans include integrating Firebase for secure user authentication and access.

Architecture
Database Layer: SQLite is utilized for local storage, featuring tables for expenses, users, budgets, and transactions.
API Layer: Retrofit manages API calls to the server for data synchronization.
Work Manager: Manages background sync operations to ensure data is updated seamlessly without interrupting the user experience.


Conclusion
This app aims to assist users in monitoring their spending habits and maintaining financial stability. By utilizing GitHub and GitHub Actions, the development process is streamlined, leading to efficient development cycles and faster delivery.


 
GitHub
The project is hosted on GitHub, which facilitates version control and collaboration. 
We use GitHub to manage code changes, track issues, and streamline the development process. 
GitHub Actions are employed to automate several tasks:
Continuous Integration (CI): Each commit initiates a build process that runs unit tests, ensuring that new changes do not disrupt existing functionality.
Continuous Deployment (CD): The application is automatically deployed to a staging server for additional testing.
Automated Sync Tests: Scheduled GitHub Actions execute sync tests to verify that the synchronization between the local database and the server functions correctly.
Key Benefits of GitHub Actions:
Automation: This reduces the manual effort required for running tests and deployments.
Monitoring: Actions provide valuable insights and logs for each build, making it easier to identify issues.
Efficiency: Builds are triggered automatically, ensuring continuous feedback throughout the development process.


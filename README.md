# DevOps-Insider-notes-by-me
Final notes by me

##Revision Class – Comprehensive Notes
1. IT Everywhere Concept
Today Information Technology (IT) exists in almost every industry.

Example: Travel booking platforms like MakeMyTrip.

Websites allow users to:

Search flights
Book hotels
Plan travel
Example workflow:

User opens the website.
Enters travel details (Delhi → Bangalore).
System processes request.
Results are shown from the database.
This shows how web applications work behind the scenes.

2. Platforms Where Applications Run
Modern applications are accessible on multiple platforms:

Website (Browser)
Android App
Apple / iOS App
All these platforms communicate with the same backend APIs.

Example API:

api.makemytrip.com/findFlights
APIs connect frontend applications to backend services.

3. 3-Tier Architecture (Most Common Web Architecture)
Example analogy: Restaurant

Restaurant	IT System
Waiter	Frontend
Kitchen	Backend
Store Room	Database
1. Frontend (Presentation Layer)
What users interact with.

Examples of technologies:

React
NextJS
Angular
Responsibilities:

User interface
User experience
Taking inputs
Showing results
Developed by: Frontend Developer

2. Backend (Application Layer)
Backend processes business logic.

Examples of technologies:

Python
Go
Rust
Java
.NET
Responsibilities:

Processing requests
Business logic
Communicating with database
Returning results to frontend
Developed by: Backend Developer

3. Database (Data Layer)
Stores application data.

Examples:

MySQL
MongoDB
PostgreSQL
Responsibilities:

Data storage
Query execution
Data retrieval
Managed by: Database Developer / DBA

4. Example Logic Execution
Example formula:

a = ? b = ?

Application calculates:

[ c = a^2 + b^2 + 2ab ]

Steps:

User enters values.
Backend processes the formula.
Result is stored in the database.
Result returned to frontend.
5. Roles in Software Development
UX Designer
Designs the user experience and layout of the application.

Responsibilities:

UI design
User flow
Screen layout
Developers
Frontend Developer
Creates UI using:

React
Angular
NextJS
Backend Developer
Creates server-side logic using:

Python
Java
.NET
Database Developer
Manages:

Data structure
Queries
Performance
6. Software Architecture
An Architect designs the system.

Types of architecture diagrams:

High Level Diagram (HLD)
Shows:

Overall system structure
Major components
Interaction between services
Example: Frontend → Backend → Database

Low Level Diagram (LLD)
Contains detailed technical information:

Server configuration
Network details
APIs
Database schema
7. Landing Zone in Cloud
In cloud environments, the architecture diagram is often called a Landing Zone.

Landing Zone includes:

Security
Backup
Disaster Recovery (DR)
Governance
Compliance
Best Practices
Purpose: Provide ready infrastructure where applications can run securely.

8. DevSecOps Engineer
A DevSecOps Engineer:

Takes developer code

Deploys it into the landing zone

Ensures:

Security
Automation
Monitoring
CI/CD
In simple terms:

Developer writes code → DevSecOps deploys and secures it.

9. Business Flow in IT Projects
Typical IT workflow:

Customer → Sales → Architect → Developers → Deployment

1. Sales / PreSales
Talks to client
Understands requirements
Prepares proposals
2. Manager
Manages project execution
Coordinates teams
3. Architect
Designs system architecture
Creates HLD and LLD
4. Developers
Build application code
5. DevOps
Deploys application
10. Important Project Documents
Functional Document
Explains:

What system should do
Features
Functional behavior
Statement of Work (SOW)
Defines:

Project scope
Timeline
Deliverables
Responsibilities
RACI Matrix
Defines responsibilities:

Term	Meaning
Responsible	Person doing the work
Accountable	Person responsible for final result
Consulted	Experts consulted
Informed	People kept updated
11. Agile Development Process
Projects are divided into smaller units called sprints.

Sprint
Duration example:

21 days
Comparison:

Time Unit	Duration
Week	7 days
Month	30 days
Sprint	~21 days
12. User Stories
Requirements are broken into user stories.

Example:

User Story:

As a user, I want to search flights so that I can book travel.

User stories are further broken into tasks.

13. Tracking Tools
Teams track work using tools like:

JIRA
Azure Boards
These tools manage:

Tasks
Bugs
Sprint progress
Developer assignments
14. Version Control (GitHub)
Developers push their code to repositories.

Example repository:

github.com/devopsinsiders/StreamFlix
Benefits:

Version control
Collaboration
Code history
CI/CD integration
15. Types of Application Architectures
1 Tier Architecture
All components in one system.

Frontend + Backend + Database

Example:

Simple apps
Streamflix example
Requires:

Only one computer
2 Tier Architecture
Structure:

Frontend + Backend Database

Used in many small systems.

3 Tier Architecture
Most modern applications.

Structure:

Frontend Backend Database

Benefits:

Scalability
Security
Separation of concerns
16. Deployment
Deployment means:

Running application code on a server.

Simple definition:

Deployment = Code ko computer par run karna.

17. Where Applications Can Be Deployed
Applications can run on:

1. Local Computer
Example: Windows machine

2. Linux Environment
Example:

Local Linux
Practice platforms
3. Cloud Platforms
Common cloud providers:

Microsoft Azure
AWS
Google Cloud
18. Middleware
Middleware connects applications with servers.

Example:

IIS (Internet Information Services)

Deployment path example:

C:\inetpub\wwwroot
Steps:

Install IIS
Copy application code to:
C:\inetpub\wwwroot
IIS serves the application.
19. DevOps Workflow
Complete DevOps flow:

Customer gives requirement
Architect designs system
Developers write code
Code pushed to GitHub
DevOps deploys application
Application runs on server/cloud
20. Key Idea of the Diagram
The diagram explains how an IT product moves from idea to deployment:

Customer → Sales → Architect → Developers → GitHub → DevOps → Server → Users

##📘 Comprehensive Notes – Business Use Case & Azure Fundamentals

2️⃣ Business Use Case Preparation

Example industries:

E-commerce
Banking
Healthcare
Education
OTT / Media

📌 Why Business Use Case Matters
Real-world clarity
Interview confidence
Architecture understanding
Not just “tool operators” but problem solvers

4️⃣ 1-Tier Application – Basics
🧩 What is a 1-Tier Application?
Application + Server in the same layer

Example:

Website hosted directly on VM
No separation of frontend/backend/database (yet)

🖥 Deployment Environments
Windows Laptop
Killercoda
Azure Cloud
5️⃣ Manual vs Automation (Very Important)
🚶 Manual First
Understand:

What is being created?
Why it is needed?
Dependencies
Manual steps build confidence & clarity

🤖 Automation Later
Automation without manual understanding = ❌ Danger

Automation tools come later:

Azure CLI
PowerShell
ARM / Bicep
Terraform
6️⃣ Imperative vs Declarative
🔹 Imperative
“How to do”

Step-by-step commands

Tools:

Azure CLI
PowerShell
🔹 Declarative
“What I want”

State-based

Tools:

ARM Templates (JSON)
Bicep
Terraform (HCL)
7️⃣ Infrastructure as Code (IaC) Tools
🔷 ARM / Bicep
Microsoft native tools
Written in JSON
Azure-specific
Code usually not available on GitHub
Used internally by Microsoft
🔷 Terraform
Open-source

Written in HCL

Developed by HashiCorp (IBM company)

Supports multi-cloud

CNCF aligned

Preferred because:

Customers don’t want vendor lock-in
Multi-cloud strategy is common
8️⃣ Cloud Account & Access Basics
☁ Cloud Entry Rule
To buy anything in cloud → Account required
Access control is mandatory
9️⃣ Authentication & Authorization (Core Concept)
🔐 Authentication
“Tu kaun hai be?”

Identity verification
Username, password, token
🔓 Authorization
“Tu karega kya?”

What actions are allowed
Controlled by roles
🔟 Azure Entra ID (Azure AD)
📛 Naming
Azure AD → Old name
Entra ID → New name
🧠 What is Entra ID?
Azure’s Identity & Access Management (IAM) system

Manages:

Users
Groups
Roles
Permissions
1️⃣1️⃣ RBAC – Role Based Access Control
RBAC = 3 Questions
1️⃣ Who? → User (Authentication)

2️⃣ What? → Role (What actions allowed)

3️⃣ Where? → Scope

🔍 Scope Levels
Management Group
Subscription
Resource Group
Resource
1️⃣2️⃣ Real-Life Examples (Very Important for Understanding)
🎬 Multiplex Example
Gate → Authentication
Ticket → Authorization
Screen access → Role-based
Lobby / Popcorn / Screen = Scope
🏠 Home Example
Husband has token
Kitchen / Bedroom access depends on role
1️⃣3️⃣ Azure Account Creation Behavior
First Azure account automatically creates:

A new Entra ID (Directory)
Directory contains:

Users
Groups
Roles
Example Users
dhondhu@tinku.com
tondu@tinku.com
tommy@tinku.com
zoie@tinku.com
1️⃣4️⃣ Azure Portal
URL: portal.azure.com

Login via Entra ID

Token-based authentication

Role decides:

What you can see
What you can create/delete

##🌩️ Cloud & Azure Fundamentals – Diagram Notes
1️⃣ What is Cloud?
Cloud means using someone else’s computer (server) over the internet instead of buying and maintaining your own.

No upfront hardware cost
Pay only for what you use
Accessible from anywhere
👉 Example: Azure, AWS, GCP

2️⃣ Azure Account & Entry Point
🔹 Azure Portal
Azure’s official website (dashboard):
https://portal.azure.com
This is where everything is created & managed:

VMs
Databases
Storage
Networking
Security
🔹 Account Creation
First step: create an Azure account

Once account is created:

Microsoft Entra ID (Azure Active Directory) is created automatically
A Subscription is also created
3️⃣ Microsoft Entra ID (Azure Active Directory)
🛡️ Guard Room Concept
Think of Entra ID as the Guard Room of a secured area (KGF example):

Real World	Azure Term
Guard Room	Entra ID
Guard Room Number	Tenant ID
Aadhaar / ID	Username & Password
Entry Check	Authentication
Area Access	Authorization
🔹 Tenant ID
Unique ID of Entra ID
Identifies your organization
Example:
0f7010fd-209e-4344-8457-043ffb37143b
➡️ Entra ID ki ID = Tenant ID

4️⃣ Authentication vs Authorization
✅ Authentication (Who are you?)
Identity verification

Example:

Aadhaar check
Username + Password
OTP / MFA
👉 “Tum andar aa sakte ho ya nahi?”

✅ Authorization (What can you access?)
Decides permission level

Example:

Sector 1 allowed
Weapon room not allowed
👉 “Andar aa gaye, par kaha tak ja sakte ho?”

5️⃣ Users in Entra ID
🔹 Example Users
Ravi Sharma → Global Admin
Bhakua Engineer
Sonam Bewafaa
Each user has:

Email ID
Role
Permissions
Example login flow:

https://login.microsoftonline.com/
→ Token Generated
→ Access portal.azure.com
6️⃣ Token-Based Access
🔐 What is a Token?
Temporary proof of authentication
Generated after successful login
Used to access Azure services securely
Flow:

User → login.microsoftonline.com
→ Token issued
→ portal.azure.com
Without token ❌ no access.

7️⃣ Subscription (KGF Zameen Example)
🏞️ Subscription = Zameen (Land)
Logical billing container

All resources live inside a subscription

Example:

₹14,000 free credits (trial)
Hierarchy:

Azure Account
 └── Entra ID (Tenant)
     └── Subscription
         └── Resources
8️⃣ Resources & Resource Access
Examples of resources:

Virtual Machines
Storage Accounts
Databases
Networking
Access depends on:

Role
Group
Subscription permissions
9️⃣ Groups (Important Rule ⚠️)
❌ Never assign permissions directly to users

✅ Best Practice:

User → Group → Role → Resource
Reason:

Easy management
Better security
Scalable
🔟 Cost & Security – Golden Rule 🏆
🌍 Duniya me do hi cheezein important hai:

💰 Cost
🔐 Security
Meter-based billing
Free tier available
Track usage carefully
1️⃣1️⃣ Meter & Free Tier Concept
🔹 Meter
Measures usage

Example:

100 units free
After that → chargeable
Examples:

Meter1 – 100 units free
Meter2 – 100 units free
Meter3 – 100 units free
1️⃣2️⃣ Cloud 1-Tier Architecture (Basic)
Single tier application

Everything hosted on cloud

Example:

One VM
One storage
One application
Used for:

Learning
Small demos
Proof of concept

1️⃣3️⃣ Real-Life Analogy Summary (KGF Model)
KGF Example	Azure
Gate	Azure Login
Guard Room	Entra ID
Guard Number	Tenant ID
ID Card	Credentials
Zameen	Subscription
Sector Access	Authorization
Chor	Unauthorized User

✅ Final Summary
Azure starts with Account
Entra ID handles identity & security
Subscription handles billing
Authentication = entry
Authorization = access control
Cost & Security are top priorities
Always use Groups, not direct users


## 📘 Azure Fundamentals – Comprehensive Notes (Based on Diagram)

### 1️⃣ What is an Azure Account?

An **Azure Account** is the starting point to use Microsoft Azure services.

* You log in using:

  * **Username**
  * **Password**
  * **OTP / MFA**
* Login URL: **portal.azure.com**
* Entry into Azure = **Authentication** 

💡 *Authentication = “Andar ghusna”*

---

### 2️⃣ Entra ID (Azure Active Directory)

Earlier called **Azure AD**, now **Microsoft Entra ID**.

* Automatically created when you create an Azure account
* Acts as the **identity system**
* Stores:

  * Users
  * Groups
  * Roles
  * Permissions
* Comes with **Free License** by default 

#### Example:

Allowed users:

* Bhakua Engineer
* Dhondhu
* Tondu
* Tinki

Login is validated using **username + password + OTP**.

---

### 3️⃣ Authentication vs Authorization (Very Important)

#### 🔐 Authentication

* Confirms **who you are**
* Example:

  * KGF gate security checking **Aadhaar / KYC**
* “Andar ghusna” 

#### 🔑 Authorization

* Confirms **what you are allowed to do**
* Example:

  * Which area inside KGF mine you can access:

    * Sector 1
    * Sector 2
    * Weapon Room 

---

### 4️⃣ Azure Hierarchy (Most Important Concept)

Azure follows a **hierarchical structure** for governance.

```
Management Group
   ↓
Subscription
   ↓
Resource Group
   ↓
Resources
```

This hierarchy helps manage:

* 🔐 Security
* 💰 Cost
* 📜 Governance & Compliance 

---

### 5️⃣ Management Group (MG)

* **Top-level container** in Azure
* Used to **group multiple subscriptions**
* Helps apply:

  * Policies
  * Role-based access (RBAC)
* A management group can have:

  * Multiple **child management groups** 

#### Tenant Root Group

* Created **automatically**
* Highest level management group
* Parent of all other management groups

---

### 6️⃣ Example Management Group Structure

```
Tenant Root Group
│
├── HR Management Group
│    ├── Recruitment Sub
│    │    └── Resource Groups
│
├── Sales Management Group
│    ├── Sales Subscription
│    ├── Ads Subscription
│
└── Dev / QA / UAT / Prod
```

* Each department gets **separate control**
* Easy cost tracking
* Strong security boundaries 

---

### 7️⃣ Subscription

* A **billing boundary**
* Contains:

  * Resource Groups
  * Azure services
* Example:

  * Rangoli Subscription
  * Sales Subscription
  * Ads Subscription 

💡 **Policies & budgets** are usually applied at subscription level.

---

### 8️⃣ Resource Group (RG)

* Logical container for Azure resources
* Resources inside RG:

  * VM
  * Storage
  * Database
  * Network
* RG helps in:

  * Easy deletion
  * Environment separation (dev/prod) 

---

### 9️⃣ Why This Hierarchy Exists?

Azure hierarchy is designed to:

* Maintain **security**
* Control **cost**
* Enforce **governance & compliance**
* Separate teams and environments 

---

### 🔟 Azure Free Tier & Meters

* Azure provides **free usage meters**
* Example:

  * Meter1: 100 units free
  * Meter2: 100 units free
  * Meter3: 100 units free 

⚠️ Warning:

> “Azure account banao, lekin credit card bigaadna mat” 😄

---

### 1️⃣1️⃣ Real-Life Analogy (KGF Example)

| Azure Concept    | KGF Analogy    |
| ---------------- | -------------- |
| Entra ID         | Aadhaar / KYC  |
| Authentication   | Entry gate     |
| Authorization    | Area access    |
| Management Group | Mine sections  |
| Subscription     | Land ownership |
| Resource Group   | Work area      |



---

### 1️⃣2️⃣ Career Roles You Can Mention on LinkedIn

* Cloud Migration & Transformation Architect
* Infrastructure Architect
* DevSecOps Architect
* FinOps Architect
* DevSecOps Specialist
* DevSecOps Consultant
* MLOps Engineer
* Build & Release Engineer
* Junior DevSecOps Engineer (Freshers)
* Network Engineer → Azure Cloud Engineer 

---

### 📌 Homework / Practice

* Create an Azure account
* Understand:

  * Entra ID
  * Management Group
  * Subscription
  * Resource Group
* Ask ChatGPT:

> “Explain Azure Management Group, Subscription and Resource Group hierarchy”

🔷 1. Azure Hierarchy (Overall Structure)

Azure ek layered structure follow karta hai — jaise company me levels hote hain.

Top → Bottom:

Entra ID → Management Group → Subscription → Resource Group → Resources

👉 Matlab:
Sab kuch ek proper structure me organize hota hai for control, billing, and access

🔐 2. Microsoft Entra ID

Isko tu identity system samajh.

👉 Ye manage karta hai:

Users (employees)
Login / authentication
Permissions (kaun kya access karega)

📌 Example:

Tu login karta hai Azure me → Entra ID check karta hai tu allowed hai ya nahi

💡 Real-world:
Company ka HR + Security system combined

🏢 3. Management Group

👉 Ye multiple subscriptions ko group karne ke liye hota hai

📌 Use case:

Ek company ke paas 10 subscriptions hain
Sabko ek rule apply karna hai (like security policy)

➡️ Management Group se ek hi baar me sab control

💡 Real-world:
Company ka Head Office jo sab departments ko control karta hai

💳 4. Subscription

👉 Ye sabse important hai — billing + resource container

📌 Har subscription:

Apna bill hota hai 💰
Apni limits hoti hain
Apni resources hoti hain

📌 Example:

Dev subscription
Production subscription

💡 Real-world:
Company ka department budget account

📦 5. Resource Group

👉 Ye ek logical container hai jisme tu resources ko group karta hai

📌 Example:
Ek app ke liye:

VM
Database
Storage

➡️ Sab ek Resource Group me

📌 Benefit:

Easy management
Easy delete (poora group delete kar sakta hai)

💡 Real-world:
Project folder 📁

⚙️ (Bonus) Resources

👉 Actual services:

VM (Virtual Machine)
Storage
Database
Networking

💡 Real-world:
Actual machines / tools

🔥 Simple Analogy (Yaad rakhne ke liye)
Azure Concept	Real Life Example
Entra ID	Employees + Login System
Management Group	Head Office
Subscription	Department Budget
Resource Group	Project Folder
Resources	Actual Machines
🧠 Final Short Summary

👉 Entra ID → Who you are
👉 Management Group → Big level control
👉 Subscription → Billing + boundary
👉 Resource Group → Organizing resources
👉 Resources → Actual services

🚀 Step-by-Step Azure Practical Lab
🧭 Step 0: Login to Azure

👉 Open:
➡️ https://portal.azure.com

Login using your account (Entra ID se authenticate hoga)

🔐 Step 1: Check / Understand Microsoft Entra ID
Search bar me type karo: Entra ID
Click → Microsoft Entra ID

👉 Yaha tu dekh sakta hai:

Users
Groups
Roles

📌 Lab Task:

"Users" → Click → Apna user dekh
(Optional) → New user create kar
🏢 Step 2: Create Management Group
Search: Management Groups
Click → Open
Click + Create

👉 Fill:

Name: DevOps-Group
Display Name: DevOps Team

Click Create

📌 Use:

Future me multiple subscriptions ko group karega
💳 Step 3: Check / Create Subscription
Search: Subscriptions
Click → Open

👉 Yaha tu dekh:

Already ek subscription hoga (Free Trial / Pay-As-You-Go)

📌 Optional:

Agar multiple environment banana hai:
Dev Subscription
Prod Subscription

💡 Note:
Free account me usually 1 hi subscription hota hai

📦 Step 4: Create Resource Group
Search: Resource Groups
Click → + Create

👉 Fill details:

Subscription: (select your subscription)
Resource Group Name: rg-devops-lab
Region: Central India (ya nearest)

Click → Review + Create → Create

✅ Done — tera first container ready

⚙️ Step 5: Create a Resource (Virtual Machine)
Search: Virtual Machines
Click → + Create → Azure Virtual Machine

👉 Fill basic details:

Resource Group: rg-devops-lab
VM Name: vm-devops-01
Region: Same as RG
Image: Ubuntu Server 22.04
Size: B1s (Free tier eligible)

👉 Authentication:

Username: azureuser
Password: (set strong password)

👉 Ports:

Allow SSH (22) ✔️

Click → Review + Create → Create

⏳ Wait 1–2 min

🔌 Step 6: Connect to VM
Go to VM
Click Connect → SSH

👉 Command milega:

ssh azureuser@<public-ip>

Run in terminal / PuTTY

🧹 Step 7: Clean Up (IMPORTANT 💰)

👉 Jab lab complete ho jaye:

Go to Resource Groups
Select: rg-devops-lab
Click Delete Resource Group

⚠️ Ye sab kuch delete kar dega (charges avoid karega)

🔥 Real Understanding Flow

Tu ne kya kiya:

Login → Entra ID use hua ✅
Subscription select kiya (billing) ✅
Resource Group banaya (container) ✅
VM create kiya (actual resource) ✅

👉 Full Azure hierarchy practical ho gaya 🎯

🧠 Pro Tips (Real DevOps Level)
Always naming convention use kar:
rg-, vm-, prod-, dev-
Separate environments:
Dev / Test / Prod
Use Resource Group for lifecycle management

🚀 Azure Networking Lab (VNet + Subnet + NSG)
🧠 Pehle Concept Samajh (1 min)

👉 VNet (Virtual Network)
= Tera private network (jaise ghar ka WiFi network)

👉 Subnet
= VNet ke andar chote parts (rooms)

👉 NSG (Network Security Group)
= Firewall (kaun andar aa sakta hai / kaun nahi)

🧪 Practical Lab Start
🌐 Step 1: Create VNet (Network)
Azure Portal → Search: Virtual Networks
Click → + Create

👉 Fill:

Name: vnet-devops
Region: Same (Central India)
Address Space: 10.0.0.0/16

👉 Next → IP Addresses section

🏠 Step 2: Create Subnet

Inside same VNet creation:

👉 Default subnet edit karo:

Subnet Name: subnet-web
Address Range: 10.0.1.0/24

👉 Add another subnet:

Name: subnet-db
Range: 10.0.2.0/24

Click → Review + Create → Create

🔥 Step 3: Create NSG (Firewall)
Search: Network Security Groups
Click → + Create

👉 Fill:

Name: nsg-web
Region: same
Resource Group: rg-devops-lab

Click Create

🔐 Step 4: Add Security Rules

Go inside NSG → Inbound Security Rules → + Add

✅ Allow SSH
Port: 22
Protocol: TCP
Action: Allow
Priority: 1000
✅ Allow HTTP (Website)
Port: 80
Protocol: TCP
Action: Allow
Priority: 1010

👉 Save

🔗 Step 5: Attach NSG to Subnet
Go to nsg-web
Click → Subnets
Click → + Associate

👉 Select:

VNet: vnet-devops
Subnet: subnet-web

Click OK

⚙️ Step 6: Create VM inside Subnet

(Important 🔥)

Go to Virtual Machines → Create
Use existing Resource Group: rg-devops-lab

👉 In Networking tab:

Virtual Network: vnet-devops
Subnet: subnet-web
NSG: Select existing → nsg-web

बाकी same as previous VM

Click → Create

🌍 Step 7: Test Connection
SSH:
ssh azureuser@<public-ip>
Test Website:
sudo apt update
sudo apt install nginx -y

👉 Browser me open:

http://<public-ip>

🎉 Nginx page dikhega → Networking working!

🚨 Real Understanding (Important)

👉 Flow kya hua:

VNet = Network bana
Subnet = Divide kiya (web/db)
NSG = Security lagayi
VM = Subnet me deploy kiya
🔥 Real DevOps Insight

❌ Agar NSG me port allow nahi → website nahi khulegi
❌ Agar wrong subnet → communication fail
❌ Agar private network → public access nahi

👉 Yehi real production issues hote hain

🧹 Clean Up (VERY IMPORTANT)

Delete:

Resource Group rg-devops-lab




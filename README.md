# 👕 HandsMen Threads Salesforce CRM Project

Welcome to the Salesforce CRM automation project for **HandsMen Threads**, a forward-thinking fashion organization. This project is built to enhance customer engagement, streamline data flow, and introduce automation across multiple touchpoints of the business using Salesforce tools and features.

---

## 🧵 Use Case

HandsMen Threads is embarking on a Salesforce implementation to improve how customer and inventory data is managed. This includes:

- ✅ Building a robust **data model** to centralize business records  
- ✅ Ensuring **data integrity** through well-configured UI and backend logic  
- ✅ Automating operations for **faster customer response** and **stock management**

### 🔄 Key Features

- **📧 Automated Order Confirmations**  
  Sends email notifications to customers post-order placement to improve communication and trust.

- **💎 Dynamic Loyalty Program**  
  Updates customer loyalty status based on purchase behavior, enabling reward distribution.

- **📦 Proactive Stock Alerts**  
  Notifies warehouse when any item stock falls below 5 units, ensuring timely restocking.

- **🕛 Scheduled Bulk Order Updates**  
  Processes bulk orders nightly, adjusting inventory and financials to maintain accurate records.

---

## 🧠 What You'll Learn

| 🔧 Skill                   | 📘 Description                                                                 |
|---------------------------|--------------------------------------------------------------------------------|
| **Data Modelling**        | Design custom objects, relationships, and fields tailored to business needs    |
| **Data Quality**          | Maintain data consistency using flows, validation rules, and automation tools |
| **Lightning App Builder** | Create intuitive and modular user interfaces                                  |
| **Record Triggered Flows**| Automate actions like emails and updates based on real-time data changes       |
| **Apex & Apex Triggers**  | Implement custom business logic                                                |
| **Asynchronous Apex**     | Perform large-scale background processing using `Batch`|

---


### 📌  Salesforce Platform Setup & Core Automation

**As a Salesforce Administrator**, I want to set up the platform with relevant data models, UI components, automation, and security features so that the business can efficiently manage operations and customer data.

---

### ✅ Deliverables

#### 1. 🔐 Salesforce Credentials Setup
- Developer Edition created
- Authenticated using Salesforce CLI (SFDX)

#### 2. 🧱 Data Management
- **Objects**: Custom objects like `Orders`, `Products`, `Customers`, `Loyalty__c` created
- **Tabs**: Tabs created for all major custom objects
- **Fields**: Custom fields like `Stock_Level__c`, `Loyalty_Status__c`, `Total_Spent__c`, etc.
- **App Manager**: Configured a Lightning App named **"HandsMen CRM"** with access to custom tabs

#### 3. ⚙️ Data Configuration
- Record Types for managing object variations
- Formula Fields for automatic calculations
- Validation Rules to ensure data accuracy

#### 4. 🔒 Data Security
- **Profiles**: Created custom profiles (e.g., Sales Rep, Warehouse Manager)
- **Roles**: Defined roles matching organizational hierarchy
- **Users**: Created users with assigned roles and profiles
- **Permission Sets**: Configured permission sets for reporting and flow access

#### 5. ✉️ Email Templates
- HTML templates for:
  - Order Confirmation
  - Loyalty Reward Notification
  - Stock Alert to Warehouse Team

#### 6. 🔁 Automation Using Flows
- **Record-Triggered Flows**:
  - On Order creation → Send confirmation email
  - On Loyalty criteria met → Update Loyalty Status
  - On stock level < 5 → Notify warehouse
- **Scheduled Flow**:
  - Runs daily at midnight to process bulk orders

#### 7. 💻 Automation Using Apex
- **Triggers**:
  - Maintain data relationships
  - Automatically adjust loyalty tier
- **Classes**:
  - Utility class to handle email dispatching
  - Logic class for purchase tracking

#### 8. ⚙️ Asynchronous Apex (Batch Jobs)
- **Batch Class**:
  - Updates inventory and financials at scale
  - Handles bulk order updates every night

## 🗂️ Project Structure

handsmen-threads-salesforce/
│
├── force-app/
│ └── main/
│ └── default/
│ ├── objects/
│ ├── classes/
│ ├── triggers/
│ ├── flows/
│ ├── layouts/
│ ├── permissionsets/
│ └── flexipages/
│
├── README.md

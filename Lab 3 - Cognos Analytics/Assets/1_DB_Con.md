# 🧠 IBM Cognos Analytics Workshop  
### Connecting to IBM DB2 via JDBC and Building a Data Module

This tutorial guides you through connecting IBM Cognos Analytics to an IBM DB2 database using JDBC, testing the connection, and creating a new data module for analytics.

---

## ⚙️ Step 1 – Open Data Server Connections
Click on **Data Server Connections** from the left navigation menu.

![](1.%20click%20data%20server.png)

---

## 🗂 Step 2 – Create a New Data Server
Click **+** to create a new connection.  
Select **DB2** as your database type, and set the tenant to **None**.

![](2.%20named%20and%20choose%20db2%20with%20tenant%20as%20none.png)

---

## 🔗 Step 3 – Copy the JDBC URL
Copy your DB2 JDBC connection URL from your IBM Cloud or database instance.  
You’ll need this in the next step.

![](3.%20copy%20paste%20url%20of%20jdbc.png)

---

## 🔐 Step 4 – Authentication Method
Choose your authentication method — typically **Prompt for username and password**.  
Then select the proper **Dispatcher**.

![](4.%20authentic%20method%20chos%20prompt%20username%20and%20id%20and%20chose%20the%20dispatchers.png)

---

## ✅ Step 5 – Test the Connection
Enter your DB2 credentials and click **Test Connection** to verify successful setup.

![](5.%20test%20the%20connections.png)

---

## 📋 Step 6 – Select Commands
Once connected, choose the relevant commands or tables to make available.

![](6.%20select%20all%20the%20commands.png)

---

## 📦 Step 7 – Load Data
Click **Load "DATA"** to import your data schema into Cognos.

![](7.%20load%20DATA.png)

---

## 🧩 Step 8 – Create a New Data Module
Navigate to **New > Data Module** to begin building your dataset.

![](8.%20new%20data%20module.png)

---

## 🧠 Step 9 – Choose Data Server & Database
Select the data server you configured and your database instance.

![](9.%20chose%20data%20server%20and%20your%20db%20instance.png)

---

## 📊 Step 10 – Select the Data You Want to Use
Finally, choose your tables or views and start modeling your data.

![](10.%20choose%20data.png)

---

## 🎉 You’re Done!
You’ve successfully connected IBM Cognos Analytics to your DB2 database and prepared a data module for analysis.

> 💡 Next Steps:  
> - Create dashboards using your new data module.  
> - Use AI Assistant to auto-generate insights.  
> - Share your module with your team for collaboration.

---

### 🧩 Workshop Info
- **Instructor:** *[Your Name / IBM Client Engineering Team]*  
- **Platform:** IBM Cognos Analytics on Cloud  
- **Database:** IBM DB2 on Cloud  
- **Objective:** Build, Connect, and Analyze data for smarter insights.

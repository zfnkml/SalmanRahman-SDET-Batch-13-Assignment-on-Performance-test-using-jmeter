## 📖 Table of Contents

1. [Performance Test using ...](#-performance-test-using-)
2. [Booking](#-booking)
   - [API Collection](#api-collection)
   - [Features](#features)
   - [Related Files](#related-files)
   - [Load Test Report](#load-test-report)
     - [Strategy](#strategy)
     - [Summary & Statistics](#summary--statistics)
   - [Stress Test Report](#stress-test-report)
     - [Strategy](#strategy-1)
     - [Summary & Statistics](#summary--statistics-1)
3. [Dmoney](#-dmoney)
   - [API Collection](#api-collection-1)
   - [Users](#users)
   - [Features](#features-1)
   - [Scenario Overview](#scenario-overview)
   - [Necessary Files](#necessary-files)
   - [How to Run](#how-to-run)

---

# 🧪 **Performance Test using ...**

![Performance Test](https://github.com/user-attachments/assets/2398409b-69b4-4f25-b74f-9b9aa759340f)

---

## 🏨 **Booking**

### 📜 API Collection  
- [Restful Booker API Documentation](https://restful-booker.herokuapp.com/apidoc/index.html)

### 🛠️ Features  
- **Auth**: Generate Token  
- **Create Booking**: Add new bookings  
- **Search**: Fetch booking details by ID  

### 📂 Related Files  
- `booking.jmx` – JMeter script for Booking tests  
- `booking-api-test-report.xlsx` – Detailed test report  

### 🧪 Load Test Report  

#### 📊 Strategy  
![Load Test Strategy](https://github.com/user-attachments/assets/1a0754c1-9571-492a-b1c5-dcc58f905ff3)

#### 📈 Summary & Statistics  
![Load Test Summary](https://github.com/user-attachments/assets/daf722f6-fe00-45ac-937d-7015fe0c1e4b)

### 🧪 Stress Test Report  

#### 📊 Strategy  
![Stress Test Strategy](https://github.com/user-attachments/assets/e86a3409-2fff-4e6a-8a6f-32f84a7f87c5)

#### 📈 Summary & Statistics  
![Stress Test Summary](https://github.com/user-attachments/assets/7bd19eb8-b6e3-4009-823e-4dd28ed6bcb4)

---

## 💰 **Dmoney**

### 📜 API Collection  
- [**User API Endpoints**](https://dmoney.roadtocareer.net/api-docs/user)  
- [**Transaction API Endpoints**](https://dmoney.roadtocareer.net/api-docs/transaction)

### 👥 Users  
- **Agent**  
- **Customer**  
- **Merchant**  

### 🛠️ Features  
- **Deposit Money**: Agents can deposit money to customer accounts.  
- **Send Money**: Customers can transfer money to other customers.  
- **Payment**: Customers can make payments to merchants.  

### 🗨️ Scenario Overview  

#### Simulated User Activities:
1. **Agents**: Perform deposits for 10 customers.  
2. **Customers**:  
   - Send money to 10 other customers.  
   - Make payments to 2 merchants.  

### 📂 Necessary Files  
- `Resources/Extra/Agent Recharge from System.csv`  
- `Resources/deposit.csv`  
- `Resources/payment.csv`  
- `Resources/sendMoney.csv`  
- `dmoney.jmx` – JMeter script for Dmoney tests  

### **🖥️ How to Run?**  
1. **Clone this Repository**:  

2. **Open `dmoney.jmx`** in JMeter.

3. **Run Agent Recharge from System**:
   - Select all 4 Thread Groups.  
   - Toggle (Ctrl + T):  
     - **Enable**: Thread Group named “Agent Recharge from System”.  
     - **Disable**: Other 3 Thread Groups.  
   - Run the script (Ctrl + R).  

4. **Run Remaining Scenarios**:
   - Select all 4 Thread Groups.  
   - Toggle (Ctrl + T):  
     - **Disable**: Thread Group named “Agent Recharge from System”.  
     - **Enable**: Other 3 Thread Groups.  
   - Run the script (Ctrl + R).  

---

![Dmoney Workflow](https://github.com/user-attachments/assets/1c2084ac-8c12-4972-86e5-786fab1111c2)

---

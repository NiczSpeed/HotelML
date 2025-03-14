# 🏨 HotelML – Documentation & Architecture  

## 📖 Table of Contents
1. [📌 Overview](#-overview)
2. [📊 System Architecture ](#-system-architecture)
3. [📂 Structure of Repositories](#-structure-of-repositories)
4. [▶️ How to Run the Entire System?](#️-how-to-run-the-entire-system)
5. [📸 Examples of Application Screenshots](#-examples-of-application-screenshots)

## 📌 Overview   
**HotelML** project was created to support the hotel infrastructure management process , developed as part of an engineering thesis. The system consists of multiple microservices that handle among other things, booking and adding rooms and hotels, the process of registering and logging users, modifying their data, creating and managing reservations.  

---

## 📊 System Architecture  
Below is a diagram showing the architecture of the system:

📌 **Architecture Diagram:** 

🔗 [View the architecture Diagram](docs/diagrams/architecture_diagram.svg)  

## 📂 Structure of Repositories
The system includes the following microservices:

| Service | Description | Repository |
|---------|------------|------------|
| 💳 **hotel_ml_front** | Application UI | [Repo](https://github.com/NiczSpeed/hotel_ml_front) |
| 🏠 **Hotel_ML_APIGateway_Service** | Central API communication hub | [Repo](https://github.com/NiczSpeed/Hotel_ML_APIGateway_Service) |
| 📦 **Hotel_ML_Auth_Service** | User data management | [Repo](https://github.com/NiczSpeed/Hotel_ML_Auth_Service) |
| 🖥️ **Hotel_ML_Rooms_And_Hotels_Service** | Hotel and room management | [Repo](https://github.com/NiczSpeed/Hotel_ML_Rooms_And_Hotels_Service) |
| 🔄 **Hotel_ML_Reservation_Service** | Reservation management | [Repo](https://github.com/NiczSpeed/Hotel_ML_Reservation_Service) |

---

## ▶️ How to Run the Entire System?  
1️⃣ **Install Docker and Docker Compose**  
2️⃣ **Clone the repositories of all microservices:**  
```sh
git clone https://github.com/NiczSpeed/hotel_ml_front
git clone https://github.com/NiczSpeed/Hotel_ML_APIGateway_Service
git clone https://github.com/NiczSpeed/Hotel_ML_Auth_Service
git clone https://github.com/NiczSpeed/Hotel_ML_Rooms_And_Hotels_Service
git clone https://github.com/NiczSpeed/Hotel_ML_Reservation_Service
```
3️⃣ **Go to the Hotel_ML_APIGateway_Service repository:**
```sh
cd Hotel_ML_APIGateway_Service
```
4️⃣ **Build Docker Images for Microservices:**
```sh
docker-compose build 
```
5️⃣ **Build and start all microservices using Docker Compose:**
```sh
docker-compose up --build 
```

6️⃣ **Go to http://localhost:8080/**

---

## 📸 Examples of Application Screenshots
### 🔹 Home Page of a Non-logged-in User
🔗 [View the home page of a non-logged-in user](docs/photos/home_page_non-logged-in_user.png)

---

### 🔹 Login Page
🔗 [View the login page](docs/photos/login_page.png)

---

### 🔹 Registration Page
🔗 [View the registration page](docs/photos/registration_page.png)

---

### 🔹 Main Menu of the Logged-in Admin
🔗 [View the main menu of the logged-in admin](docs/photos/main-menu-of-the-logged-in-admin.png)

---

### 🔹 Main Menu of the Logged-in User
🔗 [View the main menu of the logged-in user](docs/photos/main-menu-of-the-logged-in-user.png)

---

### 🔹 List of Available Rooms
🔗 [View the list of available rooms](docs/photos/list-of-available-rooms.png)
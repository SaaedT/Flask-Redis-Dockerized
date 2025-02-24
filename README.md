# Dockerized Flask & Redis App

This project demonstrates a simple web application using Flask and Redis, fully containerized with Docker and deployed on an AWS EC2 instance.

## 📌 Project Overview
The application is a minimal web service that leverages **Flask** for handling HTTP requests and **Redis** for managing state. It is deployed using **Docker Compose** for easy container orchestration.

![Project Overview](images/project_overview.png)

## 🏗️ Project Structure
```
.
├── Dockerfile
├── docker-compose.yaml
├── app.py
├── requirements.txt
```

### 🔹 `Dockerfile`
Defines the container environment for the Flask application.

![Dockerfile](images/dockerfile.png)

### 🔹 `docker-compose.yaml`
Configures the multi-container setup, linking Flask and Redis.

![Docker Compose](images/docker_compose.png)

### 🔹 `app.py`
A simple Python script handling requests and interacting with Redis.

![App.py](images/app_py.png)

### 🔹 `requirements.txt`
Specifies the required dependencies (Flask & Redis).

![Requirements](images/requirements.png)

---

## 🚀 Running the Project
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/yourusername/repository-name.git
cd repository-name
```

### 2️⃣ Build and Start the Containers
```bash
docker-compose up -d
```
This starts the application in detached mode. The web interface is accessible via:
```
http://<EC2-PUBLIC-IP>:5000
```

#### ✅ Running Containers & Directory Structure
This screenshot shows the running containers along with the project directory and images:
![Running Containers](images/running_containers.png)

### 3️⃣ Application Verification
The application was tested by refreshing the page multiple times to ensure proper session handling. Below are the screenshots showing the working interface:

#### ✅ App Running Successfully
![App Screenshot 1](images/app_screenshot_1.png)
![App Screenshot 2](images/app_screenshot_2.png)
![App Screenshot 3](images/app_screenshot_3.png)
![App Screenshot 4](images/app_screenshot_4.png)

### 4️⃣ Stopping the Application
To stop and remove the running containers, run:
```bash
docker-compose down
```
After this, the application is no longer accessible.

#### ⛔ App Stopped (Containers Removed)
![Containers Stopped](images/containers_down.png)

---

## 🛠️ Built With
- **Python** 🐍 (Flask & Redis)
- **Docker & Docker Compose** 🐳
- **AWS EC2** ☁️

## 📢 Contributing
Feel free to fork this repository, submit issues, or create pull requests!

## 📜 License
This project is licensed under the MIT License.

---

📌 **Author:** Mo Saeed Tello  
📌 **GitHub:** [yourusername](https://github.com/SaaedT)


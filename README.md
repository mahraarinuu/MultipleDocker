### **📄 README.md for Multiple-Service Docker Deployment**  

This **`README.md`** explains how to set up and run the **Multiple-Service** using **Docker** by building the image manually.  

---

# **🚀 Multiple-Service Docker Deployment**  
This project **automates the deployment of Multiple-Service in a Docker container**. The Docker image is **built locally** before running the service.  

✅ **No manual installation needed**  
✅ **Builds the image locally for full control**  
✅ **Runs in Docker for portability**  

---

## **📦 Prerequisites**  
Before running the service, ensure you have:  
- **Docker installed** → [Download Here](https://docs.docker.com/get-docker/)  
- **An internet connection** to download dependencies  

---

## **🛠️ Setup & Run**
### **1️⃣ Clone the Repository**  
```bash
git clone https://github.com/naksh-07/MultipleDocker.git
cd multiple-service
```

### **2️⃣ Create the `multi.env` File**  
This file **stores the required environment variables** for the service.  

**Example (`multi.env`):**  
```ini
BANDWIDTH_DOWNLOAD=500
BANDWIDTH_UPLOAD=250
STORAGE=10
IDENTIFIER=XXXXXXXX
PIN=XXXXXX
```

---

## **⚙️ Build & Run the Docker Image**
### **3️⃣ Build the Docker Image Locally**  
```bash
docker build -t multiple-service .
```

### **4️⃣ Run the Container**  
```bash
./run.sh
```

This script **automatically stops and removes old containers**, then **runs the new container**.

---

## **🛑 Stop & Remove the Container**
To stop and remove the running container:  
```bash
docker stop multiple-container
docker rm multiple-container
```

---

## **📜 Logs & Debugging**
To check the service logs:  
```bash
docker logs -f multiple-container
```

---

## **🎯 Expected Outcome**
- The service **builds locally** and runs in Docker  
- Environment variables from **`multi.env`** are used  
- **No need for external dependencies**  

---

### **🤝 Contributing**
Feel free to **open an issue** or **submit a pull request** if you find any improvements! 🚀  

📩 **Contact:** riyasaksena502@gmail.com  

---

🚀 **Enjoy running Multiple-Service with Docker!** 🔥🔥

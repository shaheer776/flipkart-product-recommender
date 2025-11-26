---

# **Flipkart Product Recommender System**

An intelligent, LLM-powered product recommendation system that uses customer review data to generate personalized suggestions.
This project integrates **LangChain**, **Groq API**, **HuggingFace Embeddings**, and **AstraDB Vector Database**, and is deployed as a fully containerized Flask application on **Kubernetes**, with monitoring enabled through **Prometheus** and **Grafana**.

---

##  **Project Goals**

* Build an intelligent product recommendation system using customer review data.
* Implement a **RAG (Retrieval-Augmented Generation)** workflow with vector database lookup.
* Deploy the application as a **scalable, containerized web service** using Kubernetes.
* Enable **monitoring, metrics, and observability** with Grafana and Prometheus.
* Maintain a clean, modular, production-ready codebase with logging and robust exception handling.

---

##  **Tech Stack & Tools**

### **LLM & Backend**

* Python
* LangChain
* Groq API
* HuggingFace Embeddings
* Flask (REST backend)

### **Vector Database**

* AstraDB Vector Store (DataStax)

### **Deployment & Scaling**

* Docker
* Kubernetes
* Google Cloud VM (GCE)

### **Monitoring & Observability**

* Prometheus
* Grafana

### **Code Quality**

* Modular architecture
* Custom Logging
* Custom Exception Handling

---

##  **Key Contributions**

* Designed and implemented a **RAG-based recommendation system** using LangChain, Groq API, and HuggingFace embeddings.
* Processed customer review data and indexed it into **AstraDB** for fast vector search.
* Developed a modular **Flask backend** to serve recommendations through a chatbot interface.
* Added **custom logging** and **exception handling** for robustness and maintainability.
* Containerized the entire system using **Docker** and deployed it on **Kubernetes** running on Google Cloud.
* Set up monitoring using **Prometheus metrics** and created **Grafana dashboards** for real-time observability.
* Ensured a clean architecture supporting scalability, maintainability, and production deployment.

---

## 📂 **Repository Structure**

```
flipkart-product-recommender/
│── flipkart/
│   ├── rag_chain.py
│   ├── data_ingestion.py
│   ├── data_converter.py
│   └── config.py
│
│── app.py               # Flask Backend
│── requirements.txt
│── Dockerfile
│
│── prometheus/
│   ├── prometheus-configmap.yaml
│   ├── prometheus-deployment.yaml
│
│── grafana/
│   ├── grafana-deployment.yaml
│
│── data/
│   ├── flipkart_product_review.csv
│
│── templates/
│   ├── style.css
│
│── static/
│   ├── index.html
│
│── utils/
│   ├── custom_exception.py
│   ├── logger.py
│
└── README.md
```

---

## 🔧 **How to Run Locally**

### 1️⃣ Clone the repository

```bash
git clone https://github.com/shaheer776/flipkart-product-recommender.git
cd flipkart-product-recommender
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Run the Flask backend

```bash
python app.py
```

The app will run on:

```
http://localhost:5000
```

---

## 🐳 **Docker Usage**

### Build image:

```bash
docker build -t flipkart-recommender .
```

### Run container:

```bash
docker run -p 5000:5000 flipkart-recommender
```


---

##  **Monitoring**

Prometheus collects metrics from your Flask app.
Grafana visualizes dashboard panels such as:

* API latency
* Request count
* Uptime
* Kubernetes pod status

---

## 📷 **Screenshots**

### **1. Application UI**

<img width="2560" height="1240" alt="Screenshot 2025-11-17 at 18-58-07 Chatbot" src="https://github.com/user-attachments/assets/1e141402-1c6f-4dde-863b-7d92d94098b2" />


### **2. Grafana Monitoring Dashboard**

<img width="2557" height="1240" alt="Screenshot 2025-11-17 at 19-13-52 Edit panel - New dashboard - Dashboards - Grafana" src="https://github.com/user-attachments/assets/c6a6ab01-7b8c-4aa7-9794-3a110427a373" />


### **3. Prometheus Showing Active Endpoints**

<img width="2560" height="1240" alt="Screenshot 2025-11-17 at 19-12-17 Prometheus Time Series Collection and Processing Server" src="https://github.com/user-attachments/assets/eddf859b-541e-484c-826d-8eba80d6bbbd" />


---

## ⭐ **If you like this project, please give it a star!**



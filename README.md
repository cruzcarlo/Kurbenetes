# Kubernetes Orchestration & Self-Healing Web Server

This project is a hands-on deep dive into modern infrastructure management. I moved beyond running simple Docker containers to architecting a resilient, self-healing system using **Minikube** and **kubectl**. The goal was to deploy a high-performance web server and verify that Kubernetes can maintain system uptime without manual intervention.

---

### 🛠️ Technical Execution

In this lab, I successfully implemented the following:

* **Cluster Initialization:** Configured a local Kubernetes cluster via Minikube to simulate production-grade orchestration.
* **Resource Deployment:** Created a deployment for an Nginx web server, shifting from manual container management to automated "desired state" management.
* **Service Networking:** Exposed the cluster to my local machine using a **NodePort Service**, mapping internal ports to external URLs.
* **Fault Tolerance:** Proved the platform's reliability by performing "Chaos Testing"—manually killing active processes to trigger the K8s recovery cycle.

---

### 🧪 The "Chaos Test" (Proof of Resilience)

The core value of Kubernetes is its ability to "self-heal." I verified this with a live test:
1. **Identified** the active Pod: `kubectl get pods`
2. **Triggered a failure** by deleting the Pod: `kubectl delete pod [pod-name]`
3. **Observation:** Within seconds, Kubernetes detected the missing resource and initialized a brand-new Pod automatically, ensuring zero permanent downtime.

---

### 💼 Engineering Profile

* **DevOps Mindset:** I treat infrastructure as code. From **Bash automation** to **K8s orchestration**, I focus on building systems that are scalable and reliable.
* **Full-Stack Context:** As a **BSIT student** specializing in the **MERN stack**, I understand how to bridge the gap between frontend code and the cloud infrastructure required to host it.
* **Security Focused:** My workflow incorporates best practices in **Linux permissions**, **IAM roles**, and **Security Groups** to ensure every deployment is hardened by default.
* **Continuous Learning:** I am actively mastering **CI/CD pipelines**, **Docker Networking**, and **AWS Core services** to stay adaptable in a rapidly evolving tech landscape.

### ❗ Errors 
* **I have some errors there i debug it 

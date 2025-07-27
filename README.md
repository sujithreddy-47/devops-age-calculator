# devops-age-calculator
A Java CLI Age Calculator with a complete DevOps pipeline using Git, Maven, JUnit, Jenkins, Docker, and Ansible. Includes real-time monitoring via Graphite and Grafana. Demonstrates CI/CD automation, containerization, and infrastructure as code.




````markdown
# 🧮 Age Calculator – DevOps CI/CD Project

A **Java-based CLI application** that calculates a user's age from their date of birth. This project is fully integrated into a complete **DevOps CI/CD pipeline** using modern tools: Git, Maven, JUnit, Jenkins, Docker, Ansible, and real-time monitoring with Graphite and Grafana.

---

## 📌 Project Overview

This project demonstrates how a simple Java application can be:

- Built using **Maven**
- Tested with **JUnit**
- Containerized with **Docker**
- Deployed using **Ansible**
- Automated end-to-end with **Jenkins**
- Monitored using **Graphite** and **Grafana**

It represents a realistic, production-ready CI/CD pipeline following Infrastructure-as-Code and Continuous Delivery practices.

---

## 🧰 Tech Stack

| Tool        | Purpose                                   |
|-------------|-------------------------------------------|
| Git         | Version control                           |
| Maven       | Build automation and dependency management|
| JUnit       | Unit testing                              |
| Jenkins     | Continuous integration                    |
| Docker      | Containerization                          |
| Ansible     | Deployment automation                     |
| Graphite    | Metric collection                         |
| Grafana     | Metrics visualization                     |

---

## ⚙️ How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/sujithreddy-47/devops-age-calculator.git
cd devops-age-calculator
````

### 2. Build with Maven

```bash
mvn clean install
```

### 3. Run Locally

```bash
java -jar target/age-calculator-1.0.0.jar
```

### 4. Build Docker Image

```bash
docker build -t age-calculator:latest .
```

### 5. Run Docker Container

```bash
docker run -it age-calculator:latest
```

### 6. Deploy with Ansible

Ensure Docker is running and Ansible is installed.

```bash
ansible-playbook -i hosts deploy.yml
```

### 7. Monitor with Graphite & Grafana

Start Graphite and Grafana containers.

Run the Python script to simulate metrics:

```bash
python3 metrics_simulator.py
```

Access Grafana at: [http://localhost:3000](http://localhost:3000)

Visualize the metric: `age_calculator.metrics.count`

---

## 🧪 Testing

Run JUnit tests using:

```bash
mvn test
```

Sample test in `AgeCalculatorTest.java` validates age calculation logic using fixed dates.

---

## 📦 Directory Structure

```
devops-age-calculator/
├── src/
│   ├── main/java/com/devops/age_calculator/AgeCalculator.java
│   └── test/java/com/devops/age_calculator/AgeCalculatorTest.java
├── Dockerfile
├── pom.xml
├── deploy.yml (Ansible playbook)
├── hosts (Ansible inventory)
├── metrics_simulator.py
└── README.md
```

---

## 📊 Sample Output

```
Enter your date of birth (yyyy-MM-dd): 2001-07-15
You are 24 years old.
```

---

## ✍️ Author

* **Name:** G. Sujith Reddy
* **Reg No:** 23BCE1613

---

## 🤝 Usage & Reuse

This project is open for educational and non-commercial use.
Feel free to reuse, modify, or adapt the code and CI/CD pipeline setup.
Attribution is appreciated but not required.



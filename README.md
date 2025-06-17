# 🧠 Smart News Classifier API

A modern Java + Spring Boot REST API that classifies news articles as **Real** or **Fake** using simple AI-based logic.

This project mimics a real-world AI application pipeline, with scope to integrate advanced LLMs, ML models, or external APIs later. Ideal for your resume or GitHub showcase.

---

## 🚀 Features

- ✅ REST API to submit news articles (title + content)
- ✅ Returns classification: `Real` or `Fake`
- ✅ Modular architecture (controller, service, model)
- ✅ Easily extendable for AI/ML integrations
- ✅ Clean, production-grade Spring Boot setup

---

## 🧪 Sample Request

### POST `/api/news/classify`

```json
{
  "title": "Breaking Miracle Fruit Found!",
  "content": "This miracle fruit can cure all diseases overnight, experts say."
}
```

### Sample Response:
```
"Fake"
```

---

## 📂 Project Structure

```
SmartNewsClassifierAPI/
├── controller/              # Handles HTTP requests
├── service/                # Contains business logic
├── model/                  # Request/Response models
├── SmartNewsClassifierApiApplication.java
├── resources/
│   └── application.properties
├── pom.xml                 # Maven build file
└── README.md               # Project documentation
```

---

## 🧠 AI Logic Used

Currently using **rule-based** detection. You can later:
- Connect to an LLM (e.g., GPT)
- Integrate a pre-trained ML model
- Deploy a Python microservice that classifies news

---

## 🔧 Tech Stack

| Tool         | Purpose                         |
|--------------|----------------------------------|
| Java 11      | Core language                   |
| Spring Boot  | REST API framework              |
| Maven        | Dependency management           |
| Lombok       | Boilerplate code cleanup        |
| JUnit        | Unit testing                    |

---

## ▶️ How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/SmartNewsClassifierAPI.git
   cd SmartNewsClassifierAPI
   ```

2. Run the app:
   ```bash
   mvn spring-boot:run
   ```

3. Test it via Postman or curl:
   ```bash
   curl -X POST http://localhost:8080/api/news/classify \
        -H 'Content-Type: application/json' \
        -d '{"title":"Big Miracle Found!","content":"Cures cancer instantly"}'
   ```

---

## 🛠️ Future Enhancements

- Integrate real ML/LLM prediction API
- Store results in PostgreSQL/MongoDB
- Add Swagger UI for API docs
- Add JWT Auth and logging

---

## 👨‍💻 Author

Made with  by **Mayank Sharma**

📌 Feel free to fork, star ⭐, and contribute!

---

## 📘 License

This project is open-sourced under the MIT License.

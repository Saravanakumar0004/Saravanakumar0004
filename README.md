<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=0:0d1117,100:161b22&height=150&section=header&text=saravanakumar-api&fontSize=46&fontColor=58a6ff&fontAlignY=45&desc=v1.0.0%20%7C%20Java%20Full%20Stack%20Developer%20%7C%20status%3A%20UP&descSize=16&descColor=8b949e&descAlignY=70" />

```text
  .   ____          _            __ _ _
 /\\ / ___'_ __ _ _(_)_ __  __ _ \ \ \ \
( ( )\___ | '_ | '_| | '_ \/ _` | \ \ \ \
 \\/  ___)| |_)| | | | | || (_| |  ) ) ) )
  '  |____| .__|_| |_|_| |_\__, | / / / /
 =========|_|==============|___/=/_/_/_/
 :: SaravanakumarApplication ::        (v1.0.0)

 Started SaravanakumarApplication in 0.8 seconds
 Tomcat started on port(s): 8080 (http)
 Profile active: developer | Mode: always-learning
```

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=JetBrains+Mono&weight=500&size=18&duration=3000&pause=800&color=58A6FF&center=true&vCenter=true&width=780&lines=GET+%2Fapi%2Fdeveloper+%E2%86%92+200+OK;POST+%2Fapi%2Fprojects+%E2%86%92+201+Created;Building+REST+APIs+that+scale;docker+build+%26%26+kubectl+apply+%E2%86%92+deployed+%F0%9F%9A%80" alt="API typing" />
</p>

<p align="center">
  <a href="https://saravanakumar-portfolio-sable.vercel.app/"><img src="https://img.shields.io/badge/Portfolio-58a6ff?style=flat-square&logo=vercel&logoColor=black" /></a>
  <a href="https://www.linkedin.com/in/saravanakumar1912/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:saravanakumars3019@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/Build-passing-3fb950?style=flat-square" />
  <img src="https://img.shields.io/badge/Open_to_work-yes-3fb950?style=flat-square" />
  <img src="https://komarev.com/ghpvc/?username=Saravanakumar0004&label=Requests&color=58a6ff&style=flat-square" />
</p>

---

## 📋 `GET /actuator/health`

```json
{
  "status": "UP",
  "developer": "Saravanakumar S",
  "role": "Java Full Stack Developer",
  "education": "B.Tech - Computer Science & Business Systems",
  "components": {
    "backend":  { "status": "UP", "details": ["Java", "Spring Boot", "Node.js", ".NET"] },
    "frontend": { "status": "UP", "details": ["React", "JavaScript", "HTML", "CSS"] },
    "database": { "status": "UP", "details": ["MySQL", "MongoDB"] },
    "devops":   { "status": "UP", "details": ["Git", "Docker"] },
    "learning": { "status": "IN_PROGRESS", "details": ["Microservices", "Kubernetes", "AWS"] }
  }
}
```

---

## ⚙️ `application.yml`

```yaml
developer:
  name: Saravanakumar S
  role: Java Full Stack Developer
  focus:
    - REST API Development
    - Database Design
    - Clean Architecture
    - System Design
  goal: Build scalable products used by millions
  motto: "Code. Learn. Build. Repeat."

server:
  port: 8080

contact:
  email: saravanakumars3019@gmail.com
  open-to-work: true
```

---

## 🔌 API Endpoints

| Method | Endpoint | Description | Status |
|:--:|:--|:--|:--:|
| `GET` | `/api/developer/skills` | Java, Spring Boot, React, Node.js, .NET, MySQL, MongoDB | ![200](https://img.shields.io/badge/200-OK-3fb950?style=flat-square) |
| `GET` | `/api/developer/projects` | 6 full stack and IoT projects (listed below) | ![200](https://img.shields.io/badge/200-OK-3fb950?style=flat-square) |
| `POST` | `/api/developer/hire` | Open to Java Full Stack and Backend roles | ![201](https://img.shields.io/badge/201-Created-58a6ff?style=flat-square) |
| `PUT` | `/api/developer/skills/learning` | Microservices, Docker, Kubernetes, AWS | ![202](https://img.shields.io/badge/202-Updating-d29922?style=flat-square) |

---

## 🏛 Layered Architecture I Follow

```mermaid
sequenceDiagram
    autonumber
    participant C as React Client
    participant CT as Controller
    participant S as Service
    participant R as Repository
    participant DB as MySQL / MongoDB

    C->>CT: HTTP Request + JWT
    CT->>CT: Validate input
    CT->>S: Call business logic
    S->>R: Fetch / Save data
    R->>DB: Query
    DB-->>R: Result
    R-->>S: Entity
    S-->>CT: DTO
    CT-->>C: JSON Response
```

---

## 🗄 Typical Database Design

```mermaid
erDiagram
    USER ||--o{ ROLE : has
    USER ||--o{ PROJECT : manages
    PROJECT ||--o{ TASK : contains
    USER ||--o{ TASK : assigned

    USER {
        int id PK
        string name
        string email
        string password
    }
    ROLE {
        int id PK
        string role_name
    }
    PROJECT {
        int id PK
        string title
        string status
    }
    TASK {
        int id PK
        string description
        date due_date
    }
```

---

## 🚀 Project Modules

| # | Module | Tech Focus | Key Features |
|:--:|:--|:--|:--|
| 1 | **CRM for Engineering Works** | Full Stack | Employee and client management, project tracking, auth and roles |
| 2 | **IoT IV Infusion Monitoring** | IoT + Web | Real-time fluid monitoring, alerts, sensor integration |
| 3 | **Campus Lost & Found Portal** | Web | Student login, report, search and claim items |
| 4 | **Agro Connect** | Web | Farmer-to-customer marketplace, direct buyer communication |
| 5 | **Smart Waste Management** | Web + Data | Bin monitoring dashboard, data visualization |
| 6 | **Decentralized Blood Donor App** | Web + Security | Secure auth, blood search, emergency notifications |

---

## 🐳 Deployment Pipeline (Learning)

```dockerfile
# Dockerfile
FROM eclipse-temurin:17-jre
WORKDIR /app
COPY target/app.jar app.jar
EXPOSE 8080
ENTRYPOINT ["java", "-jar", "app.jar"]
```

```bash
docker build -t saravanakumar/app:1.0 .
docker run -p 8080:8080 saravanakumar/app:1.0
kubectl apply -f deployment.yaml
```

---

## 📜 `git log --oneline` (Learning Path)

```text
a1f4c92 (HEAD -> main) Learning: AWS Cloud
7be03d1 Learning: Kubernetes orchestration
c92e8a7 Learning: Docker containerization
4d1b6f0 Learning: Microservices architecture
9e3a7c5 Built: Spring Boot REST APIs with JWT
2f8d1b4 Built: React full stack applications
b6c0e93 Started: Java, OOP and DSA
```

---

## 📊 Metrics

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=Saravanakumar0004&show_icons=true&theme=github_dark&hide_border=true&count_private=true" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Saravanakumar0004&layout=compact&theme=github_dark&hide_border=true" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=Saravanakumar0004&theme=github-dark-blue&hide_border=true" />
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Saravanakumar0004&theme=github-compact&hide_border=true" />
</p>

---

## 🛠 Dependencies (`pom.xml` style)

<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,react,nodejs,express,dotnet,html,css,js,bootstrap,mysql,mongodb,git,github,docker,kubernetes,postman,swagger,vscode,visualstudio&perline=10" />
</p>

---

## 📫 `POST /api/contact`

```http
POST /api/contact HTTP/1.1
Host: saravanakumar-portfolio-sable.vercel.app
Content-Type: application/json

{
  "to": "saravanakumars3019@gmail.com",
  "linkedin": "linkedin.com/in/saravanakumar1912",
  "message": "Let's build something scalable together."
}
```

<img width="100%" src="https://capsule-render.vercel.app/api?type=rect&color=0:161b22,100:0d1117&height=80&section=footer" />

# 🩺 Backend de l'application Healthrack

> **Healthrack** est une application personnelle de suivi et d’analyse des indicateurs de santé — notamment le **taux de glucose**, le **poids** et la **tension artérielle**.  
> Ce projet est né de mon envie de mieux comprendre mes données de santé au quotidien, grâce à une interface simple et des visualisations claires.

---

## 🚀 Stack technique

### 🧠 Backend
- **Langage :** Golang  
- **Framework :** [Gin](https://github.com/gin-gonic/gin)  
- **ORM :** [GORM](https://gorm.io)  
- **Base de données :** PostgreSQL (ou autre, selon configuration)  
- **Tests :** `testing` + `httptest`


## 📂 Structure du projet

Healthrack_api/
│
├── backend/
│ ├── main.go # points d'entree
│ ├── go.mod  #dependence
│ ├── handlers/
│ ├── entity/
| ├── dto/
| ├── midllewares/
| ├── db/ #config database
| ├── repository/ #interface avec la base de donnees
| ├── service/   
| ├── controller/
| ├── handler/#config des endpoints ou routes
| ├── server/#SetupRouter 
| ├── /test #contient les tests unitaires
│ └── .env/# config connexion environnement 
| ├── dockerfile #config de docker




Configuration
#  Crée un fichier .env
App_Env="Production"
PORT=9090
DB_HOST=localhost
DB_PORT=5432
DB_USER=postgres
DB_PASSWORD=secret
DB_NAME=healthrack


---

## ⚙️ Installation & exécution

### 1️⃣ Cloner le dépôt
```bash
git clone https://github.com/Senitdev/healthtrack_api.git
cd healthtrack_api
go mod tidy
go run main.go

#Le backend est disponible sur http://localhost:9090

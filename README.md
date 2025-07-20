# Application SpringBoot BDCC AI

Ce projet est une application Spring Boot intégrant le framework expérimental [Spring AI](https://github.com/spring-projects/spring-ai) pour construire une application multimodale basée sur des agents d'IA. Elle met en avant les fonctionnalités suivantes :

- Interactions en langage naturel avec des agents IA.
- Traitement d'image en texte.
- Génération d'images à partir de prompts textuels.
- Prise en charge de plusieurs types de modèles IA via différents endpoints.

## 📁 Structure du Projet
```
main/
├── java/ma/enset/bdccai/
│   ├── BdccAiApplication.java         # Main Spring Boot application
│   ├── controllers/                   # Controllers for REST endpoints
│   ├── outputs/                       # POJOs for structured outputs
├── resources/
│   ├── application.properties         # Spring config
│   ├── images/                        # Sample images for testing
```


## 🚀 Fonctionnalités

- **/chat** – Interaction en langage naturel avec un agent IA.
- **/streaming** – Réponses de chat en streaming.
- **/structured** – Réponses JSON structurées pour formats prédéfinis comme les films ou les cartes d'identité (CIN).
- **/image/generate** – Génération d'une image à partir d'une description textuelle.
- **/describe** – Retourne une description textuelle d’une image fournie en utilisant un modèle multimodal.

## 🔧 Instructions d'installation

### Prérequis

- Java 21
- Maven
- Spring Boot 3.x ou supérieur
- Accès à un fournisseur de modèles IA supporté (ex : OpenAI, Hugging Face, ou modèles locaux)
- Connexion Internet pour l’appel aux API de modèles (sauf si inférence locale utilisée)

### Installation

```bash

Lancement de l'application

mvn spring-boot:run
Accès aux API
Une fois lancée, l'application expose les endpoints suivants :


GET http://localhost:8899/chat
GET http://localhost:8899/describe
POST http://localhost:8899/image/generate
Utilisez des outils comme Swagger ou Postman pour tester ces endpoints.
```
---
## 📦 Dépendances

Spring Boot

Spring AI (expérimental)

Librairies clients OpenAI/HuggingFace

---
## 🧠 Auteur

Mouad Dacheikh
# 📚 MongoDB CRUD Application

Welcome to MongoDB CRUD Application! 🎉 

This project is a RESTful API developed with Spring Boot that uses MongoDB as its database. It allows CRUD operations (Create, Read, Update, Delete) on a collection of tutorials. It's perfect for learning about the integration between Spring Boot and MongoDB.

## 📋 API Endpoints

Our API provides the following endpoints:

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET    | /api/tutorials | Get all tutorials or search by title |
| GET    | /api/tutorials/{id} | Get a tutorial by its ID |
| POST   | /api/tutorials | Create a new tutorial |
| PUT    | /api/tutorials/{id} | Update a tutorial by its ID |
| DELETE | /api/tutorials/{id} | Delete a tutorial by its ID |
| DELETE | /api/tutorials | Delete all tutorials |

### 📥 Creating a Tutorial

To create a new tutorial, use the POST /api/tutorials endpoint with a JSON body like this:

```json
{
  "title": "Learning Spring Boot",
  "description": "Complete guide to Spring Boot",
  "published": true
}

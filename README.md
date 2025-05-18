# Getting Started

First build the project
mvn compile
mvn package

# Run the application either using jar or mvn command
java -jar target/azure-mongodb-crud-0.0.1-SNAPSHOT.jar
or
mvn spring-boot:run

# Perform CRUD operation either using postman or curl commands
curl -X POST -H "Content-Type: application/json" -d '{"description": "Create a new task", "severity": 1, "assignee": "John Doe", "storyPoint": 5}' http://localhost:8080/tasks
curl -X GET http://localhost:8080/tasks
curl -X GET http://localhost:8080/tasks/{$taskId}
curl -X PUT -H "Content-Type: application/json" -d '{"description": "Update task description", "severity": 2, "assignee": "Jane Doe", "storyPoint": 10}' http://localhost:8080/tasks/1
curl -X DELETE http://localhost:8080/tasks/1

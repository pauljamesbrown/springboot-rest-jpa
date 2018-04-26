This is a simple springboot rest app that stores notes in a database.

The following methods have be implemented:

- createNote
- updateNote
- deleteNote
- getAllNotes
- getNote

To run type: mvn spring-boot:run

To test:

- createNote
curl -d '{"title" : "Note 1", "content" : "random data"}' -H "Content-Type: application/json" -X POST http://localhost:8080/api/notes

- updateNote
curl -d '{"title" : "Note 1 change to note 2", "content" : "random data"}' -H "Content-Type: application/json" -X PUT http://localhost:8080/api/notes/1

- deleteNote
curl -H "Content-Type: application/json" -X DELETE http://localhost:8080/api/notes/1

- getNote
curl -H "Content-Type: application/json" -X GET http://localhost:8080/api/notes/2

- getAllNotes

curl -H "Content-Type: application/json" -X GET http://localhost:8080/api/notes
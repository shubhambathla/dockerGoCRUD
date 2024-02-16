# How to test the CRUD APIs

```bash
curl -X GET http://localhost:8012/tasks
curl -X POST http://localhost:8012/tasks \\n-H "Content-Type: application/json" \\n-d '{"title": "Study for exams", "status":"pending"}'
curl -X GET http://localhost:8012/tasks
curl -X PUT http://localhost:8012/task/75e37821-a30a-4242-966f-63a0bb22bf8b -H "Content-Type: application/json" -d '{"title": "Study for exams", "status":"complete"}'
curl -X GET http://localhost:8012/tasks
```
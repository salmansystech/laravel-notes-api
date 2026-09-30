# API Testing Guide

## Testing with cURL

### Get all notes
```bash
curl http://localhost:8000/api/notes
```

### Create a note
```bash
curl -X POST http://localhost:8000/api/notes \
  -H "Content-Type: application/json" \
  -d '{"title":"My Note","body":"Note content"}'
```

### Get specific note
```bash
curl http://localhost:8000/api/notes/1
```

### Update a note
```bash
curl -X PUT http://localhost:8000/api/notes/1 \
  -H "Content-Type: application/json" \
  -d '{"title":"Updated","body":"New content"}'
```

### Delete a note
```bash
curl -X DELETE http://localhost:8000/api/notes/1
```

# Example Usage

## GET All Students
```bash
curl http://localhost/project1/code/api/students.php

## POST Create Student 
curl -X POST http://localhost/project1/code/api/students.php \
  -H "Content-Type: application/json" \
  -d '{"first_name":"Alice","last_name":"Brown","email":"a@email.com"}'

## POST Enrollment (Secured)
  curl -X POST http://localhost/project1/code/api/enrollments.php \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer test_token_12345abcdef" \
  -d '{"student_id":1,"course_id":1}'

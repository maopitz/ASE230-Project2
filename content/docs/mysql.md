# Database Structure

## Database: `student_management`

### Tables:
- `students`  
- `courses`  
- `enrollments`  
- `api_tokens`  

### ER Diagram (text description)

**students**
- id (PK)
- first_name
- last_name
- email
- enrollment_date

**courses**
- id (PK)
- course_code
- course_name
- credits
- instructor

**enrollments**
- id (PK)
- student_id (FK → students.id)
- course_id (FK → courses.id)
- UNIQUE(student_id, course_id)

**api_tokens**
- id (PK)
- token
- user_type
- expires_at

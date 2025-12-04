# API Security

## Bearer Token Authentication
All enrollment routes require a Bearer token.

### Workflow:
1. Client sends token using `Authorization: Bearer TOKEN`
2. Server:
   - Validates token format
   - Checks it against the `api_tokens` database table
   - Ensures token not expired
3. If valid → request continues  
4. If invalid → 401 Unauthorized

## Why tokens?
- Simple and effective for teaching REST concepts  
- Works well with shell scripts, Postman, and JS fetch  
# poscirle-project

## I. API Specification

### 1. **POST /auth/login**

- **Request Body**:
  ```json
  {
    "email": "string",
    "password": "string"
  }
  ```
  
- **Res Body**:
     ```json
    {
       "id": "string",
       "name": "string",
       "email": "string"
     }
     ```
     
### POST /auth/register
- **Req Body**:
   ```json
   {
      "name": "string",
      "email": "string",
      "password": "string"
   }
   ```
- **Res Body**:
   ```json
   {
      "message": "string"
   }
   ```

### POST /posts
- **Req Body**:
   ```json
   {
      "title": "string",
      "content": "string",
      "author": {"name": "string"}
   }
   ```
   - **Res Body**:
   ```json
   {
      "message": "string"
   }
   ```

## GET /home 
- **Res Body**:
   ```json
   {
      "data": [
         {"id": "string",
         "title": "string",
         "content": "string",
         "author": {"name": "string"}
         }
      ]
   }
   ```

## GET /home/pencarian 
- **Req Body**:
   ```json{
      "name": "string",
   }
   ```
   - **Res Body**:
   ```json{
      "data": [
         {"name": "string",
          "email": "string" 
         }
      ]
   }
   ```

# API Documentation

This documentation provides details on how to use the PHP REST API for managing person records.

## Endpoints

### Create a Person

**Endpoint:** `POST /api` ```https://splendidabbey.afobe.net/api```

**Request Body:**

```json
{
  "name": "John Doe",
  "age": 30,
  "email": "johndoe@example.com"
}
```

### Get Person Details
**Endpoint:** `GET /api/{id}` ```https://splendidabbey.afobe.net/api/1```

Response Example:
```json
{
  "id": 1,
  "name": "John Doe",
  "age": 30,
  "email": "johndoe@example.com"
}
```

### Update Person Details
**Endpoint:** `PUT /api/{id}` ```https://splendidabbey.afobe.net/api/1```

Request Body:
```json
{
  "name": "Updated Name",
  "age": 35
}
```

### Delete a Person
**Endpoint:** `DELETE /api/{id}` ```https://splendidabbey.afobe.net/api/1```

### Dynamic Parameter Handling
You can use the name parameter to filter persons by name. For example, if you want to perform CRUD operations on a person named "John Doe," you can provide the name in the request.

### Error Handling
The API returns appropriate error responses for invalid requests, missing parameters, and database errors.

### Testing
You can run automated tests using PHPUnit. See the README for instructions on running tests.

### License
This project is licensed under the MIT License - see the LICENSE file for details.


Feel free to customize these templates to fit your project's specific details and requirements.

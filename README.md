# REST-API-
from basic CRUD


1.What you understand by CRUD
CRUD stands for Create, Read, Update, and Delete. It represents the basic operations that can be performed on data in a persistent storage system, such as a database. These operations are fundamental in most software applications for managing and manipulating data.

2.Create a REST endpoint for each above operation.
Create - POST /users
Read - GET /users/{id}
Update - PUT /users/{id}    # Full update
               PATCH /users/{id}  # Partial update
Delete - DELETE /users/{id}

3. Update can be done via PUT and PATCH. What the difference on each.
PUT:
Used for updating a resource or creating a new resource if it doesn't exist.
Requires sending the complete representation of the resource in the request.
If a field is not provided in the request, it is typically set to null or a default value.

PATCH:
Used for making partial updates to a resource.
Requires sending only the data that needs to be updated, rather than the complete representation of the resource.
Allows for more efficient updates by transmitting only the changes.

# Introduction to SOLID

This will be an application for listing and registering users. For user listing to work, the user requesting the listing must be an admin (more details in the description).

## Controllers and Use Cases:

### POST `/users`

-[X] The route must receive `name`, and `email` inside the request body so that it is possible to register a user.

### PATCH `/users/:user_id/admin`

-[X] The route must receive, in the route parameters, the `id` of a user and transform this user into admin.

### GET `/users/:user_id`

-[X] The route must receive, in the route parameters, the `id` of a user and return the user information found by the response body.

### GET `/users`

-[X] The route must receive, via the request header, a `user_id` property containing the `id` of the user and return a list of all registered users. The `id` should be used to validate if the user requesting the listing is an admin. Returning the list should only be done if the user is admin.

## Models
-[X] Create user model

## Repository
-[X] Implement create user logic

-[X] Implement logic to list all users

-[X] Implement logic to find a user by id

-[X] Implement logic to find a user by email

-[X] Implement logic to make a user as admin


## Documentation
- Access the documentation at http://localhost:3333/api-docs/#/

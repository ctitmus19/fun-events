---
layout: page
---

# Get users
Using the Fun Events API, you can get a list of all users that belong to the API database.

Before beginning the tutorial, make sure to [test your development system](../tutorials/getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

## Table of contents
- [Get users with cURL commands](#curl)
- [Get users in Postman](#Postman)

---
## <a name="curl">Get users with cURL commands</a>

Using your preferred command line tool, complete the following steps:

1. Ensure that the fun-events JSON file is running in a command line tool
2. In a separate command line tool, enter the following:
```shell
curl {base_url}/users
```
3. Submit the command.
4. View the JSON response:
```shell
[
  {
    "last_name": "Button",
    "first_name": "Benjamin",
    "email": "b.button@example.com",
    "id": 1
  },
  {
    "last_name": "Jones",
    "first_name": "Coraline",
    "email": "c.jones@example.com",
    "id": 2
  },
  {
    "last_name": "Parker",
    "first_name": "Peter",
    "email": "p.parker@example.com",
    "id": 3
  },
  {
    "last_name": "Skellington",
    "first_name": "Sally",
    "email": "s.skellington@example.com",
    "id": 4
  }
]
```
---
## <a name="Postman">Get events in Postman</a>

Open the Postman app on your desktop and complete the following steps:

1. Ensure that the fun-events JSON file is running in a command line tool.
2. Create a new request with the following values:
- **Method:** GET
- **URL:** {base_url}/users
- **Headers:**
  - **Content-Type:** application/json
 
3. Select the **Send** button.
4. View the JSON response:
```shell
[
  {
    "last_name": "Button",
    "first_name": "Benjamin",
    "email": "b.button@example.com",
    "id": 1
  },
  {
    "last_name": "Jones",
    "first_name": "Coraline",
    "email": "c.jones@example.com",
    "id": 2
  },
  {
    "last_name": "Parker",
    "first_name": "Peter",
    "email": "p.parker@example.com",
    "id": 3
  },
  {
    "last_name": "Skellington",
    "first_name": "Sally",
    "email": "s.skellington@example.com",
    "id": 4
  }
]
```

## Additional resources

* [User resources](user.md)
* [Get events](get-events.md)

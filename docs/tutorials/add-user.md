---
layout: page
---

# Add user
This tutorial describes how to add a new user to the Fun Events Service API. In order to complete this tutorial, you need to use the Postman application.

Before beginning the tutorial, make sure to [test your development system](../tutorials/getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

---
## Add user in Postman

Open the Postman app on your desktop and complete the following steps:

1. Create a new request with the following values:
- **Method:** POST
- **URL:** {base_url}/users
- **Headers:**
  - Content-Type: application/json
- **Request body:** Update the content below to match your user details:
```shell
  {
    "last_name": "Fletcher",
    "first_name": "Mundungus",
    "email": "m.fletcher@example.com"
  }
```

2. Select the **Send** button 
3.  View the JSON response:
```shell
{
    "last_name": "Fletcher",
    "first_name": "Mundungus",
    "email": "m.fletcher@example.com",
    "id": 5
}
```
## Additional resources

* [User resource](api/user.md)
* [Update user](update-user.md)
* [Delete user](delete-user.md)

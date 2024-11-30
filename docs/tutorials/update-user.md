---
layout: page
---

# Update user
This tutorial describes how to update a user in the Fun Events Service API. In order to complete this tutorial, you need to use the Postman application.

Before beginning the tutorial, make sure to [test your development system](getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

---
## Update user in Postman

Open the Postman app on your desktop and complete the following steps:

1. First, find the `user_id` of the user you want to update. Create a request in Postman with the following values:
- **Method:** GET
- **URL:** {base_url}/user
- **Headers:**
    - **Content-Type:** application/json

2. Locate the user you want to update
3. Find the `id` parameter and copy the ID number
4. Create a new request with the following values, with the `user_id` included at the end of the URL:
- **Method:** PUT
- **URL:** {base_url}/users/2
- **Headers:**
    - **Content-Type:** application/json
- **Request body:** Update the content below to match your event details:
```shell
 {
    "last_name": "Jones",
    "first_name": "Coraline Q.",
    "email": "c.jones@mailtime.com",
    "id": 2
  }
```

5. Select the **Send** button 
6.  View the JSON response:
```shell
{
    "last_name": "Jones",
    "first_name": "Coraline Q.",
    "email": "c.jones@mailtime.com",
    "id": 2
}
```
## Additional resources

* [User resource](../api/event.md)
* [Add user](add-user.md)
* [Delete user](delete-user.md)


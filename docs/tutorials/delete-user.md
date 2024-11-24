---
layout: page
---

# Delete user
This tutorial describes how to delete an existing user in the Fun Events Service API. To delete a user, you first need to locate the user's ID number. The steps to complete this tutorial require using the Postman application.

Before beginning the tutorial, make sure to [test your development system](getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

---
## Delete user in Postman

Open the Postman app on your desktop and complete the following steps:

1. First, find the `user_id` of the user you want to delete. Create a request in Postman with the following values:
- **Method:** GET
- **URL:** {base_url}/users
- **Headers:**
    - **Content-Type:** application/json

2. Locate the user you want to delete
3. Find the `id` parameter and copy the ID number
4. Create a new request with the following values, with the `user_id` included at the end of the URL :
- **Method:** DELETE
- **URL:** {base_url}/users/5
- **Headers:**
    - **Content-Type:** application/json

5. Select the **Send** button 
6.  View the JSON response:
```shell
{}
```
## Additional resources

* [User resource](../api/user.md)
* [Add user](add-user.md)
* [Update user](update-event.md)

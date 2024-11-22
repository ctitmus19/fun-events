---
layout: page
---

# Delete event
This tutorial describes how to delete an existing event in the Fun Events Service API. In order to delete an event, you first need to locate the event's ID number. The steps to complete this tutorial require using the Postman application.

Before beginning the tutorial, make sure to [test your development system](../tutorials/getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

---
## Delete event in Postman

Open the Postman app on your desktop and complete the following steps:

1. First, find the `event_id` of the event you want to delete. Create a request in Postman with the following values:
- **Method:** GET
- **URL:** {base_url}/events
- **Headers:**
    - **Content-Type:** application/json

2. Locate the event you want to delete
3. Find the `id` parameter and copy the ID number
4. Create a new request with the following values, with the `event_id` included at the end of the URL :
- **Method:** DELETE
- **URL:** {base_url}/events/6
- **Headers:**
    - **Content-Type:** application/json

5. Select the **Send** button 
6.  View the JSON response:
```shell
{}
```
## Additional resources

* [Event resource](api/event.md)
* [Add user](add-user.md)
* [Delete event](delete-event.md)

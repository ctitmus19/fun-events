---
layout: page
---

# Delete event
This tutorial describes how to delete an existing event in the Fun Events Service API. In order to delete an event, you first need to locate the event's ID number. The steps to complete this tutorial require using the Postman application.

Before beginning the tutorial, make sure to [test your development system](getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

---
## Delete event in Postman

Open the Postman app on your desktop and complete the following steps:

1. Ensure that the fun-events JSON file is running in a command line tool.
2. Find the `event_id` of the event you want to delete. Create a request in Postman with the following values:
- **Method:** GET
- **URL:** {base_url}/events
- **Headers:**
    - **Content-Type:** application/json

3. Locate the event you want to delete.
4. Find the `id` parameter and copy the ID number.
5. Create a new request with the following values, with the `event_id` included at the end of the URL :
- **Method:** DELETE
- **URL:** {base_url}/events/6
- **Headers:**
    - **Content-Type:** application/json

6. Select the **Send** button. 
7.  View the JSON response:
```shell
{}
```
## Additional resources

* [Event resource](../api/event.md)
* [Add event](add-event.md)
* [Delete event](delete-event.md)
---
layout: page
---

# Update event
This tutorial describes how to update an event in the Fun Events Service API. In order to complete this tutorial, you need to use the Postman application.

Before beginning the tutorial, make sure to [test your development system](getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

---
## Update event in Postman

Open the Postman app on your desktop and complete the following steps:

1. First, find the `event_id` of the event you want to update. Create a request in Postman with the following values:
- **Method:** GET
- **URL:** {base_url}/events
- **Headers:**
    - **Content-Type:** application/json

2. Locate the event you want to delete
3. Find the `id` parameter and copy the ID number
4. Create a new request with the following values, with the `event_id` included at the end of the URL:
- **Method:** PUT
- **URL:** {base_url}/events/3
- **Headers:**
  - Content-Type: application/json
- **Request body:** Update the content below to match your event details:
```shell
  {
    "user_id": 3,
    "name": "Spider-Man in Concert",
    "url": "https://seattlesymphony.org/events/spider-man",
    "description": "Listen to the Seattle Symphony perform tracks from the iconic Spider-Man movies.",
    "start_date": "2025-03-30T19:00",
    "end_date": "2025-03-30T21:00",
    "address": "200 University St",
    "city": "Seattle",
    "region": "Washington",
    "country": "United States",
    "price": 70,
    "id": 3
  }
```

5. Select the **Send** button 
6.  View the JSON response:
```shell
{
    "user_id": 3,
    "name": "Spider-Man in Concert",
    "url": "https://seattlesymphony.org/events/spider-man",
    "description": "Listen to the Seattle Symphony perform tracks from the iconic Spider-Man movies.",
    "start_date": "2025-03-30T19:00",
    "end_date": "2025-03-30T21:00",
    "address": "200 University St",
    "city": "Seattle",
    "region": "Washington",
    "country": "United States",
    "price": 70,
    "id": 3
}
```
## Additional resources

* [Event resource](../api/event.md)
* [Add event](add-event.md)
* [Delete event](delete-event.md)

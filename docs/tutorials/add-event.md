---
layout: page
---

# Add event
This tutorial describes how to add a new event to the Fun Events Service API. In order to complete this tutorial, you need to use the Postman application.

Before beginning the tutorial, make sure to [test your development system](getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

---
## Add event in Postman

Open the Postman app on your desktop and complete the following steps:

1. Ensure that the fun-events JSON file is running in a command line tool.
2. Create a new request with the following values:
- **Method:** POST
- **URL:** {base_url}/events/
- **Headers:**
  - Content-Type: application/json
- **Request body:** Update the content below to match your event details:
```shell
 {
      "user_id": 1,
      "name": "The Nutcracker",
      "url": "https://www.saltlakecountyarts.org/events/the-nutcracker-2/",
      "description": "The Nutcracker Ballet performed in 2 acts with dancers from UDI who are between the ages of 2-18, along with dancers from the University of Utah.",
      "start_date": "2024-11-21T19:00",
      "end_date": "2024-11-23T19:00",
      "address": "2525 Taylorsville Blvd",
      "city": "Taylorsville",
      "region": "Utah",
      "country": "United States",
      "price": 20
 }
```

3. Select the **Send** button. 
4.  View the JSON response:
```shell
{
    "user_id": 1,
    "name": "The Nutcracker",
    "url": "https://www.saltlakecountyarts.org/events/the-nutcracker-2/",
    "description": "The Nutcracker Ballet performed in 2 acts with dancers from UDI who are between the ages of 2-18, along with dancers from the University of Utah.",
    "start_date": "2024-11-21T19:00",
    "end_date": "2024-11-23T19:00",
    "address": "2525 Taylorsville Blvd",
    "city": "Taylorsville",
    "region": "Utah",
    "country": "United States",
    "price": 20,
    "id": 6
}
```
## Additional resources

* [Event resource](../api/event.md)
* [Add user](add-user.md)
* [Delete event](delete-event.md)
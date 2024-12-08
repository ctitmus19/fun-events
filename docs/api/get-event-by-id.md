---
layout: page
---

# Get event by ID
You can use cURL commands or Postman to retrieve information about an event if you have that event's unique ID. Use the steps below to complete this task.

Before beginning the tutorial, make sure to [test your development system](../tutorials/getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

## Table of contents
- [Get events with cURL commands](#curl)
- [Get events in Postman](#Postman)

---
## <a name="curl">Get events with cURL commands</a>

Using your preferred command line tool, complete the following steps:

1. Ensure that the fun-events JSON file is running in a command line tool.
2. In a separate command line tool, enter the following information with the last number being the `event-id` of the event you want to find:
```shell
curl http://localhost:3000/events/1
```
3. Submit the command.
4.  View the JSON response:
```shell
{
  "user_id": 1,
  "name": "Albuquerque Film Festival",
  "url": "https://abq-film/festival",
  "description": "Watch independent films submitted by people around the globe!",
  "start_date": "2025-02-22",
  "end_date": "2025-02-23",
  "address": "3701 Scenic St",
  "city": "Albuquerque",
  "region": "New Mexico",
  "country": "United States",
  "price": 30,
  "id": 1
}
```
---
## <a name="Postman">Get events in Postman</a>

Open the Postman app on your desktop and complete the following steps:

1. Ensure that the fun-events JSON database is running in a command line tool.
2. Create a new request with the following values with the last number of the URL being the `event-id` of the event you want to find:
- **Method:** GET
- **URL:** {base_url}/events/1
- **Headers:**
  - **Content-Type:** application/json

3. Select the **Send** button.
4.  View the JSON response:
```shell
  {
    "user_id": 1,
    "name": "Albuquerque Film Festival",
    "url": "https://abq-film/festival",
    "description": "Watch independent films submitted by people around the globe!",
    "start_date": "2025-02-22",
    "end_date": "2025-02-23",
    "address": "3701 Scenic St",
    "city": "Albuquerque",
    "region": "New Mexico",
    "country": "United States",
    "price": 30,
    "id": 1
  }
```
## Additional resources

* [Get all events](get-events.md)
* [Get event by user ID](get-event-by-user_id.md)
* [Get event by ID](get-event-by-id.md)
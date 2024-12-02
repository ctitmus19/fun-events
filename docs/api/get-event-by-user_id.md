---
layout: page
---

# Get event by user ID
Using the Fun Events API, you can get a list of all events associated with a specific user ID number. Follow the steps in this article to complete this task.

Before beginning the tutorial, make sure to [test your development system](../tutorials/getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

## Table of contents
- [Get events with cURL commands](#curl)
- [Get events in Postman](#Postman)

---
## <a name="curl">Get events with cURL commands</a>

Using your preferred command line tool, complete the following steps:

1. Ensure that the fun-events JSON file is running in a command line tool
2. Find the `user_id` of the user you want to update. Create a request in a separate command line tool with the following values:
```shell
curl {base_url}/users
```
2. In the response, locate the user
3. Find the `id` parameter and copy the ID number
4. In a separate command line tool, enter the following information with the `user_id` at the end:
```shell
curl {base_url}/events?user_id=1
```
5. Submit the command
6. View the JSON response:
```shell
[
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
]
```
---
## <a name="Postman">Get events in Postman</a>

Open the Postman app on your desktop and complete the following steps:

1. Ensure that the fun-events JSON database is running in a command line tool.
2. Find the `user_id` of the user you want to update. Create a request in Postman with the following values:
- **Method:** GET
- **URL:** {base_url}/user
- **Headers:**
    - **Content-Type:** application/json

3. Locate the user.
4. Find the `id` parameter and copy the ID number.
5. Create a new request with the following values, with the `user_id` included at the end of the URL:
6. Create a new request with the following values:
- **Method:** GET
- **URL:** {base_url}/events?user_id=1
- **Headers:**
  - Content-Type: application/json
 
7. Select the **Send** button.
8. View the JSON response:
```shell
[
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
]
```
## Additional resources

* [Get all events](get-events.md)
* [Get event by ID](get-event-by-id.md)
* [Get event by date range](get-events-by-date-range.md)
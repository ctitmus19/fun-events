---
layout: page
---

# Get event by user ID
Using the Fun Events API, you can get a list of all events associated with a specific user ID number. Follow the steps in this article to complete this task.

Before beginning the tutorial, make sure to [test your development system](../tutorials/getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`

**Time to complete:** 5 minutes

---
## Get events with cURL commands

Using your preferred command line tool, complete the following steps:

1. Ensure that the fun-events JSON file is running in a command line tool
2. In a separate command line tool, enter the following:
```shell
curl {base_url}/events?user_id=1
```
3. Replace `1` with the ID number of the user whose events you want to retrieve
4. Submit the command
5. View the JSON response:
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
## Get events in Postman

Open the Postman app on your desktop and complete the following steps:

1. Create a new request with the following values:
- **Method:** GET
- **URL:** {base_url}/events?user_id=1
- **Headers:**
  - Content-Type: application/json
 
2. In the URL, replace `1` with the ID number of the user whose events you want to retrieve
3. Select the **Send** button
4. View the JSON response:
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

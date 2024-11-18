---
layout: page
---

# Get events
Using the Fun Events API, you can get a list of all events that belong to the API database.

Before beginning the tutorial, make sure to [test your development system](../tutorials/getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

---
## Get events with cURL commands

Using your preferred command line tool, complete the following steps:

1. Ensure that the fun-events JSON file is running in a command line tool
2. In a separate command line tool, enter the following:
```shell
curl {base_url}/events
```
3. Submit the command
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
  },
  {
    "user_id": 2,
    "name": "Dahlia Society Showcase",
    "url": "https://dahlia-society/showcase",
    "description": "Admire dahlias grown by members of the Vancouver Dahlia Society!",
    "start_date": "2025-03-29T13:00",
    "end_date": "2025-03-29T15:00",
    "address": "1600 Floral Rd",
    "city": "Vancouver",
    "region": "British Columbia",
    "country": "Canada",
    "price": 0,
    "id": 2
  },
...
]
```
---
## Get events in Postman

Open the Postman app on your desktop and complete the following steps:

1. Create a new request with the following values:
- **Method:** GET
- **URL:** {base_url}/events
- **Headers:**
  - Content-Type: application/json
 
2. Select the **Send** button
3. View the JSON response:
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
  },
  {
    "user_id": 2,
    "name": "Dahlia Society Showcase",
    "url": "https://dahlia-society/showcase",
    "description": "Admire dahlias grown by members of the Vancouver Dahlia Society!",
    "start_date": "2025-03-29T13:00",
    "end_date": "2025-03-29T15:00",
    "address": "1600 Floral Rd",
    "city": "Vancouver",
    "region": "British Columbia",
    "country": "Canada",
    "price": 0,
    "id": 2
  },
...
]
```
## Additional resources

* [Event resource](event.md)
* [Get users](get-users.md)
* [Get event by ID](get-event-by-id.md)
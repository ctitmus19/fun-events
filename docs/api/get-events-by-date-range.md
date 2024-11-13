---
layout: page
---

# Get events by date range
Using the Fun Events Service API, you can retrieve a list of any events within a specific date range.
Use the steps in this tutorial to complete the task.

Before beginning the tutorial, make sure to [test your development system](../tutorials/getting-started.md).

**Time to complete:** 5 minutes

---
## Get events in Postman

Open the Postman app on your desktop and complete the following steps:

1. Create a new request with the following values:
- **Method:** GET
- **URL:** {base_url}/events
- **Headers:**
  - Content-Type: application/json

2. Add the following information to the end of the request URL ({base_url}/events):
```shell
?start_date_gte=YYYY-MM-DD&end_date_lte=YYYY-MM-DD
```
3. Update the date information to match your request. For example, if you want to display events between
March 21 and March 31, the request URL should look like this:
```shell
http://localhost:3000/events?start_date_gte=2025-03-21&end_date_lte=2025-03-31
```
4. Select the **Send** button

5. View the JSON response:
```shell
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
    {
        "user_id": 3,
        "name": "Spider-Man Concert",
        "url": "https://seattlesymphony.org/events/spider-man",
        "description": "Listen to the Seattle Symphony perform soundtracks from the iconic spider-man films!",
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

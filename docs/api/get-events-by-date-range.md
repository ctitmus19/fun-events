---
layout: page
---

# Get events by date range
Using the Fun Events Service API, you can retrieve a list of any events within a specific date range.
Use the steps in this tutorial to complete the task.

Before beginning the tutorial, make sure to [test your development system](../tutorials/getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5-10 minutes

## Table of contents
- [Get events with cURL commands](#curl)
- [Get events in Postman](#Postman)

---
## <a name="curl">Get events with cURL commands</a>

Using your preferred command line tool, complete the following steps:

1. Ensure that the fun-events JSON database is running in a command line tool.
2. In a separate command line tool, enter the following but **do not submit the command**:
```shell
curl "{base_url}/events?start_date_gte=YYYY-MM-DD&end_date_lte=YYYY-MM-DD"
```
3. Update the date information to match your request. For example, if you want to display events between
March 21 and March 31, the request URL should look like this:
```shell
curl "{base_url}/events?start_date_gte=2025-03-21&end_date_lte=2025-03-31"
```
4. Submit the command.
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
---
## <a name="Postman">Get events in Postman</a>

Open the Postman app on your desktop and complete the following steps:

1. Ensure that the fun-events JSON database is running in a command line tool.
2. Create a new request with the following values:
- **Method:** GET
- **URL:** {base_url}/events
- **Headers:**
  - Content-Type: application/json

3. Add the following information to the end of the request URL ({base_url}/events), but **do not submit the request** :
```shell
?start_date_gte=YYYY-MM-DD&end_date_lte=YYYY-MM-DD
```
4. Update the date information to match your request. For example, if you want to display events between
March 21 and March 31, the request URL should look like this:
```shell
{base_url}/events?start_date_gte=2025-03-21&end_date_lte=2025-03-31
```
5. Select the **Send** button

6. View the JSON response:
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
## Additional resources

* [Get all events](get-events.md)
* [Get event by ID](get-event-by-id.md)
* [Get event by user ID](get-event-by-user_id.md)
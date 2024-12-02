---
layout: page
---

# Get events by location
Using the Fun Events Service API, you can retrieve a list of any events that take place in a specific location. There are four location properties: `address`, `city`, `region` (typically the state or province), and `country`. This article describes how to retrieve events by `city`, `region`, and `country`.

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
2. In a separate command line tool, enter the following, but **do not submit the command**:
### City
```shell
curl {base_url}/events?city="Seattle"
```
### Region
```shell
curl {base_url}/events?region="Washington"
```
### Country
```shell
curl {base_url}/events?country="United States"
```

3. Update the location information to match your desired request. For example, replace "Seattle" with "Los Angeles" or "San Francisco".
4. Submit the command.
5. View the JSON response:
```shell
[
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
  },
  {
    "user_id": 4,
    "name": "Halloween Party",
    "url": "https://seattle.gov/events/halloween-party",
    "description": "Celebrate spooky season!",
    "start_date": "2025-10-31T17:00",
    "end_date": "2025-10-31T20:00",
    "address": "1031 Hallow Ave",
    "city": "Seattle",
    "region": "Washington",
    "country": "United States",
    "price": 5,
    "id": 4
  }
]
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

3. Add the following information to the end of the request URL ({base_url}/events), but **do not submit the request**:

### City
```shell
?city="Seattle"
```
### Region
```shell
?region="Washington"
```
### Country
```shell
?country="United States"
```

4. Update the date information to match your request. For example, replace "Seattle" with "Los Angeles" or "San Francisco".
5. Select the **Send** button.

6. View the JSON response:
```shell
[
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
  },
  {
    "user_id": 4,
    "name": "Halloween Party",
    "url": "https://seattle.gov/events/halloween-party",
    "description": "Celebrate spooky season!",
    "start_date": "2025-10-31T17:00",
    "end_date": "2025-10-31T20:00",
    "address": "1031 Hallow Ave",
    "city": "Seattle",
    "region": "Washington",
    "country": "United States",
    "price": 5,
    "id": 4
  }
]
```
## Additional resources

* [Get all events](get-events.md)
* [Get event by date range](get-events-by-date-range.md)
* [Get event by user ID](get-event-by-user_id.md)

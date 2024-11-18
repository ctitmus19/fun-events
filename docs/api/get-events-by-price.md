---
layout: page
---

# Get events by price
Using the Fun Events Service API, you can retrieve a list of any events that are either less than or greater than a specific price. Use the steps in this tutorial to complete the task.

Before beginning the tutorial, make sure to [test your development system](../tutorials/getting-started.md).

**Note:** Typically, the `{base_url}` used in commands is `http://localhost:3000`.

**Time to complete:** 5 minutes

---
## Get events with cURL commands
### Events less than specific price
Using your preferred command line tool, complete the following steps:

1. Ensure that the fun-events JSON file is running in a command line tool
2. In a separate command line tool, enter the following:
```shell
curl "{base_url}/events?price_lte=15
```
3. Update the price information to match your request. For example, if you want to display events with a price lower than $10, replace `price_lte=15` with `price_lte=10`

4. Submit the command
5. View the JSON response:
```shell
[
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
### Events greater than specific price
Using your preferred command line tool, complete the following steps:

1. Ensure that the fun-events JSON file is running in a command line tool
2. In a separate command line tool, enter the following:
```shell
curl "{base_url}/events?price_gte=25
```
3. Update the price information to match your request. For example, if you want to display events with a price higher than $10, replace `price_gte=25` with `price_gte=10`

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
]
```
---
## Get events in Postman
### Events less than specific price
Open the Postman app on your desktop and complete the following steps:

1. Create a new request with the following values:
- **Method:** GET
- **URL:** {base_url}/events?price_lte=15
- **Headers:**
  - Content-Type: application/json

2. Update the price information to match your request. For example, if you want to display events with a price lower than $10, replace `price_lte=15` with `price_lte=10`

3. Select the **Send** button

4. View the JSON response:
```shell
[
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

### Events greater than specific price
Open the Postman app on your desktop and complete the following steps:

1. Create a new request with the following values:
- **Method:** GET
- **URL:** {base_url}/events?price_gte=25
- **Headers:**
  - Content-Type: application/json

2. Update the price information to match your request. For example, if you want to display events with a price greater than $10, replace `price_gte=25` with `price_gte=10`

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
]
```

## Additional resources

* [Get all events](get-events.md)
* [Get events by location](get-events-by-location.md)
* [Get events by date range](get-events-by-date-range.md)
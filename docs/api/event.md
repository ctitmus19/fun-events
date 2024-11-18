---
layout: page
---

# `event` resource

Base endpoint:

```shell

{server_url}/events
```

Contains information about events added to the service.

To advertise an event in the service, the user must be added to
the service first. Learn more about the [user resource](user.md).

## Resource properties

Sample `event` resource

```js

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

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `user_id` | number | The ID of the user who created the event |
| `name` | string | The title of the event |
| `url` | string | The website where additional event information can be found |
| `description` | string | Short description of the event |
| `start_date` | number | The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format for the start date and time of the event|
| `end_date` | number | The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format for the end date and time of the event |
| `address` | string | The street address for the event |
| `city` | string | The city where the event will take place |
| `region` | string | The state or province where the event will take place |
| `country` | string | The country where the event will take place |
| `price` | number | The cost of the event
| `id` | number | The event's unique record ID

## Additional resources

* [Get all events](get-events.md)
* [Get event by ID](get-event-by-id.md)
* [Get event by user ID](get-event-by-user_id.md)

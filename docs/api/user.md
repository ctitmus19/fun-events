---
layout: page
---

# `user` resource

Base endpoint:

```shell

{server_url}/users
```

Contains information about users in the service.

After a user has been created, they can be associated with any created event in the service. Learn more about the [event resource](event.md).

## Resource properties

Sample `user` resource

```js

   {
      "last_name": "Jones",
      "first_name": "Coraline",
      "email": "c.jones@example.com",
      "id": 2
    }
```

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `last_name` | string | The last name of the user |
| `first_name` | string | The first name of the user |
| `email` | string | The email address of the user |
| `id` | number | The user's unique record ID

## Additional information

* [Get all users](get-users.md)
* [Add user](tutorials/add-user.md)
* [Update user](tutorials/update-user.md)

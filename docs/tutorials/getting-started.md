---
layout: page
---

# Getting started with Fun Events API

Before you can run the **Fun Events Service API**, you must download the required tools and
test your development system.

Time for completion: About 20 minutes

## Download required tools

To utilize the **Fun Events Service API**, you need the following tools:
**Note:** You may want to open the links in separate broswer tabs.

* A [GitHub account](https://github.com)
* A development system (PC, Mac, or Linux) running a current or
long-term support (LTS version of the operating system).
* The following software on your development system:
    * [Git](https://docs.github.com/en/get-started/quickstart/set-up-git) (for the command line)
    * [GitHub Desktop](https://desktop.github.com) (optional)
    * A fork of the [fun-events repo](https://github.com/ctitmus19/fun-events)
    * A current/LTS version of `node.js`
    * A current version of [json-server](https://www.npmjs.com/package/json-server)
    * A current copy of the database file. You can get this by syncing your fork.
    * The [Postman desktop app](https://www.postman.com/downloads/). Because you run the **Fun Events Service API** on your development system with an `http://localhost` hostname, the web-version of Postman can't perform the exercises.

## Test development system

Complete the following steps to test your development system:

1. Create and checkout a test branch of your fork of the To-Do-service repo. Your `GitHub repo workspace` is the directory that contains your fork of the `fun-events` repo.

    ```shell
    cd <your GitHub repo workspace>
    ls
    # (see the fun-events directory in the list)
    cd fun-events
    git checkout -b tutorial-test
    cd api
    json-server -w events-db-source.json
    ```

    If your development system is installed correctly, you should see
    the service start and display the URL of the service: `http://localhost:3000`.

2. Make a test call to the service.

    ```shell
    curl http://localhost:3000/users
    ```

3. If the service is running correctly, you should see a list of users from the service, such as in this example:

    ```js
    [
        {
    "last_name": "Button",
    "first_name": "Benjamin",
    "email": "b.button@example.com",
    "id": 1
  },
  {
    "last_name": "Jones",
    "first_name": "Coraline",
    "email": "c.jones@example.com",
    "id": 2
  },
        ...
    ```

If the list of users does not display or you receive an error,
 investigate and correct the error before continuing.

 Complete the following steps to search for errors:
1. Review each command for any errors.
2. Ensure you are in the correct directory.
3. Make sure that required software components installed correctly.
4. Verify that required software components are up to date.

If you see the list of users from the service, you're ready to begin using the **Fun Events Service API**.
View the [Tutorials](tutorials.md) for more possible actions you can try.

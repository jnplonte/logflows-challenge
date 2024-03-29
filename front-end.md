# LOGFLOWS Software Engineer Challenge - Frontend

- [Overview](#overview)
- [Functional Requirements](#functional-requirements)
- [Other Requirements](#other-requirements)
- [Frameworks and Libraries](#frameworks-and-libraries)
- [Using the Mock API](#using-the-mock-api)
- [Implementation Notes](#implementation-notes)
- [Wireframes](#wireframes)

## Overview

the application should allow the user to view, create, update and delete user information and joborders.


## Functional Requirements

1. as a user i need to view user and joborders with embedded map using [Google Maps](https://developers.google.com/maps/) from the list of user information.
2. as a user i need to update a user and add joborder from the list of user information.
3. as a user i need to add a user from the list of user information.
4. as a user i need to delete a user from the list of user information.

*NOTE: please do not include your google API key in your submission. Instead use a configurable config file to store the api key.*


## Other Requirements

1. major functionalities should be cover on the test.
2. support for modern browsers.
3. instructions and `readme.md` on how to use the application should be included.
4. use of git.
5. end to end test is strong bonus

## Frameworks and Libraries

we mainly use VueJs at LOGFLOWS, however you are free to use whatever framework that you are familiar with (vue/react/angular).


## Using the Mock API

The Mock API has been deployed at [https://61f2aba52219930017f5080b.mockapi.io](https://61f2aba52219930017f5080b.mockapi.io)


- Method: `GET` - get all users
  - URL path: `/users`

- Method: `GET` - get specific user
  - URL path: `/users/<:id>`
  
- Method: `POST` - insert user
  - URL path: `/users`
  - Sample Request body:

    ```
    {
      "name": "Peter Parker",
      "image": "https://cloudflare-ipfs.com/ipfs/Qmd3W5DuhgHirLHGVixi6V76LhCkZUz6pnFt5AJBiyvHye/avatar/800.jpg",
      "companyName": "logflows",
      "email": "spiderman@gmail.com",
      "remarks": "remarks 1",
      "jobOrders": [
          {
              "pickup": {
                  "latitude": 22.335538,
                  "longitude": 114.176169,
                  "address": "Kowloon Tong"
              },
              "dropoff": {
                  "latitude": 22.319181,
                  "longitude": 114.170008,
                  "address": "Mong Kok"
              }
          }
      ]
  	}
    ```
    
- Method: `PUT` - update user
  - URL path: `/users/<:id>`
  - Sample Request body:

    ```
    {
      "name": "Bruce Wayne"
      "email": "batman@gmail.com"
  	}
    ```
    
- Method: `DELETE` - delete specific user
  - URL path: `/users/<:id>`

## Implementation Notes

- you can work on your own schedule, but a complete solution is expected within 14 days.
- your code should be modular. Each module should focus on doing one thing well.
- you must be frugal in the use of third-party libraries. (don’t include a 300 KB library just for one helper function)
- you can implement any additional features that you think will enhance the user experience.

## Wireframes

these wireframes serve as a reference for the UI of your application. You can be creative with UI/UX and additional features.

[wireframe](https://xd.adobe.com/spec/a1516e48-56fb-4e40-739e-cf27bcd00d47-d760/)



**Questions? Suggestions? Ping us at: [johnpaul@logflows.com](mailto:johnpaul@logflows.com)**

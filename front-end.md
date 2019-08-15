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
3. as a user i need to add a user from the list of user information..
4. as a user i need to delete a user from the list of user information.

*NOTE: please do not include your google API key in your submission. Instead use a configurable config file to store the api key.*


## Other Requirements

1. major functionalities should be cover on the test.
2. support for modern browsers.
3. Instructions and readme on how to use the application should be included and must be production ready.
4. use of git.
5. end to end test is strong bonus

## Frameworks and Libraries

we mainly use VueJs at LOGFLOWS, however you are free to use whatever framework or library that you are familiar with or prefer.


## Using the Mock API

The Mock API has been deployed at [https://5adff6ee17a03000145b2551.mockapi.io/v1](https://5adff6ee17a03000145b2551.mockapi.io/v1).


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
      "image": "https://s3.amazonaws.com/uifaces/faces/twitter/bighanddesign/128.jpg",
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

- You can work on your own schedule, but a complete solution is expected within 14 days.
- Your code should be modular. Each module should focus on doing one thing well.
- We aim for reusable components and a maintainable codebase.
- Be frugal in the use of third-party libraries. (don’t include a 300 KB library just for one helper function)
- You can implement any additional features that you think will enhance the user experience.

## Wireframes

these wireframes serve as a reference for the UI of your application. You can be creative with UI/UX and additional features.

xxxxxxxxxxxxxxxxxxx TO FOLLOW WIREFRAMES xxxxxxxxxxxxxxxxxxx



**Questions? Suggestions? Ping us at: [johnpaul@logflows.com](mailto:johnpaul@logflows.com)**

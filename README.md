# Social-Network-Api
A social network web application where users can share their thoughts, react to friends’ thoughts, and create a friend list. You’ll use Express.js for routing, a MongoDB database, and the Mongoose ODM. In addition to using the Express.jsLinks to an external site. and MongooseLinks to an external site. packages, you may also optionally use a JavaScript date library of your choice or the native JavaScript Date object to format timestamps.

## User Story

AS A social media startup \
I WANT an API for my social network that uses a NoSQL database \
SO THAT my website can handle large amounts of unstructured data

## Acceptance Criteria

GIVEN a social network API \
WHEN I enter the command to invoke the application \
THEN my server is started and the Mongoose models are synced to the MongoDB database \
WHEN I open API GET routes in Insomnia Core for users and thoughts \
THEN the data for each of these routes is displayed in a formatted JSON \
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core \
THEN I am able to successfully create, update, and delete users and thoughts in my database \
WHEN I test API POST and DELETE routes in Insomnia Core \
THEN I am able to successfully create and delete reactions to thoughts and add and remove friends to a user’s

## Languages + Technologies Used
- Express js
- Mongo Db


## Tests


On Insomnia, the following API routes have been created and used to add, update, or remove users, friends, thoughts, and reactions in the user's database.

📁 **USER**

- Create a new user: `POST /api/users`
- Get all users: `GET /api/users`
- Get a single user by its `id`: `GET /api/users/:userId`

- Update a user by its `id`: `PUT /api/users/:userId`

- Delete a user by its `id`: `DELETE /api/user/:userId`

📁 **FRIEND**

- Add a new friend to a user's friend list: `POST /api/users/:userid/friends/:friendId`
- Delete a friend from a user's friend list: `DELETE /api/users/:userid/friends/:friendId`

📁 **THOUGHT**

- Create a new thought: `POST /api/thoughts/`
- Get all thoughts: `GET /api/thoughts/`
- Get a single thought by its `id`: `GET /api/thoughts/:thoughtId`
- Update a thought by its `id`: `PUT /api/thoughts/:thoughtId`
- Delete a thought by its `id`: `DELETE /api/thoughts/:thoughtId`

📁 **REACTION**

- Create a reaction: `POST /api/thoughts/:thoughtId/reactions`
- Delete a reaction by the `reactionId`: `DEL /api/thoughts/:thoughtId/reactions/:reactionId`

[![Walkthrough Video](https://img.youtube.com/vi/YqyOhSHBa5w/0.jpg)](https://www.youtube.com/watch?v=YqyOhSHBa5w)
# DevConnector - Restful API Server

DevConnector is a social network for developers built with Node.js, Express and MongoDB. This repository includes RESTful API server code of DevConnector. It allows users to get the list of all registered developers, profile of each developer, and provides CRUD functionality for post, comment and like.

## Quick Start

#### 1) Clone the repository

```
$ git clone https://github.com/minashin/devconnector-backend.git
```

#### 2) Install dependencies

```
$ cd devconnector-backend
$ npm install
```

#### 3) Modify default.json

You will need to create a default.json in the config folder with

```
{
  "mongoURI": "YOUR_MONGO_URI",
  "jwtSecret": "YOUR_JWT_SECRET"
}
```

#### 4) Run server

```
$ npm run backend
```

## REST API Routes

#### Users:

| Route          | Description     |
| -------------- | --------------- |
| POST api/users | Register a user |

#### Profile:

| Route               | Description                   |
| ------------------- | ----------------------------- |
| GET api/profile     | Get all profiles              |
| POST api/profile    | Create or update user profile |
| DELETE api/profile  | Delete user profile           |
| GET api/profile/me  | Get current user profile      |
| GET api/profile/:id | Get profile by user id        |

#### Auth:

| Route         | Description         |
| ------------- | ------------------- |
| GET api/auth  | Get a user by token |
| POST api/auth | Authenticate a user |

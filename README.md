# Cordia API

This is the backend side of a real-time groupal chat app, based on discord, which I made purely as an academical project

[Frontend Repository](https://github.com/chrisdadev/Cordia)

[Live Demo]("https://cordia.vercel.app") :point_left:

## Endpoints

### Users

| Description     | Method | URL                  |
| --------------- | ------ | -------------------- |
| Register        | POST   | /api/users/register  |
| Login           | POST   | /api/users/login     |
| Get user        | GET    | /api/users/user      |
| Get user groups | GET    | /api/users/getGroups |

### Groups

| Description           | Method | URL                            |
| --------------------- | ------ | ------------------------------ |
| Create                | POST   | /api/groups/createGroup        |
| Join                  | POST   | /api/groups/joinGroup          |
| Get group information | GET    | /api/groups/groupData/:id/:jwt |

## Technologies used

- [TypeScript](https://www.typescriptlang.org/)
- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
- [MongoDB](https://www.mongodb.com/)
- [Mongoose](https://mongoosejs.com/)
- [JWT](https://jwt.io/)

## Getting started

### Clone repository

```
git clone https://github.com/chrisdadev13/Cordia-API.git
cd Cordia-API
```

### Set up environment variables

```
PORT=<The port the server will run on, e.g. 8000>
DB_ADMIN=<Database username>
DB_PASSWORD=<Database password>
DB_NAME=<Database name or direction>
SECRET_TOKEN=<Secret used to sign the session ID cookie>
```

### Install packages and start server

```
npm i
npm run start
```

### Authentication

For users authentication I used JWT tokens which are stored on client side as local storage (accessToken).

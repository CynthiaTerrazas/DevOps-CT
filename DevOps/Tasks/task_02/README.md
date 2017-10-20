# DevOps-CT
AT-04 DevOps

# RESTful API project with Nodejs, Express and MongoDB.

## Installation

- Clone the repo: 

`git clone https://github.com/AT-04/DevOps-CT.git`

- Install dependencies with the following command: 

`npm install`

- to run the database run the following command:

```js
"C:\Program Files\MongoDB\Server\3.4\bin\mongod.exe"
```

- to start the server run the following command:

`npm run start`  

- The server will start at: http://localhost:3000

## RESTful API endpoint and services.

### POST `/tasks`

Create a new task.

For create a new task the name is requiered.

+ Method: `POST`
+ URL: `/tasks`
+ Body:

```js
{
 "name": "task01",
 "status": "pending"
}

```


### GET `/tasks`

Get all tasks.

+ Method: `GET`
+ URL: `/tasks`

### GET `/tasks/:taskId`

Get task by specific id.

+ Method: `GET`
+ URL: `/tasks/59e8a55976473c17b8f04471`

### PUT `/tasks/:taskId`

Update task by specific id.

+ Method: `PUT`
+ URL: `/tasks/59e8a55976473c17b8f04471`
+ Body:

```js
{
"name": "task02",
 "status": "finished"
}

```


### DELETE `/tasks/:taskId`

Delete task by specific id.

+ Method: `DELETE`
+ URL: `/tasks/59e8a55976473c17b8f04471`
+ Body contains the message:

```js
{
    "message": "Task successfully deleted"
}

```
# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup

**[TODO 05/01/2018 @vanessa-cooper]:** _It's been a while since anyone ran a fresh copy of this repo. I think it's worth documenting the steps needed to install and run the repo on a new machine?_

The first thing we need to do is clone this repo. To do that, copy the repository url and run following command:
```
$ git clone <repo_url>
```

Now open this repo in any text editor / ide of your choice. 

Before running this, we need to [install docker](https://docs.docker.com/get-docker/).  
Confirm that docker is installed by running
```
$ docker -v
```

Now we can load-up the container from project root by executing:
```
$ docker-compose up
```

This command will install all the dependencies of the container on the first run, so it may take a little time. When the container is running, we can check it by using the `http://localhost:3000/api/ping` api by opening it in the browser.


Let's start by creating a new user at `http://localhost:3001/register` to check if everything is working fine. If it's created successfully, we can move on to next steps!

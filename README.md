# Instaclone Backend

Instagram clone using MERN stack

This is the backend repo built with Express and MongoDB. If you looking for the frontend repo, [click here](https://github.com/manikandanraji/instaclone-frontend)

[Check out the deployed site](https://merninsta.netlify.app)

## Running Locally

At the root of the project, you should have a .env with the following contents

```js
JWT_SECRET=<yoursupersecret>
JWT_EXPIRE=30d // or anything you prefer
MONGOURI=<your_mongodb_connection_uri>
```

Then run <code>npm i && npm run dev</code> to start the development server

## Deploying the backend to heroku

First create an heroku account and install the heroku cli globally and login

```bash
npm i -g heroku
heroku login
```

Once logged in, create a new heroku application and push it to the remote 'heroku'

```bash
heroku create
git push heroku master
```
Then we need to manually setup the environmental variables using the heroku dashboard

## Deploying Backend to Railway.app

Click the button below to deploy, please change the JWT secret and change some code to refer to the MONGODB plugin they offer, If you don't want to change much, then after deploy find the mongodb connection url and make another ENV_var and add that.

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new?template=https%3A%2F%2Fgithub.com%2Fmanikandanraji%2Finstaclone-backend&plugins=mongodb&envs=JWT_SECRECT%2CJWT_EXPIRE&JWT_SECRECTDesc=Secret+Key+For+JWT&JWT_EXPIREDesc=When+would+the+JWT+tokens+expire&JWT_SECRECTDefault=VERY-SECURE-KEY&JWT_EXPIREDefault=30d)

## UI

### Home 
![Home](screenshots/home_new.png)

### Explore
![Explore](screenshots/explore_new.png)


### Followers
![Followers](screenshots/followers_new.png)


### Profile
![Profile](screenshots/profile_new.png)

### Edit Profile
![Edit Profile](screenshots/edit_profile_new.png)

### New Post
![New Post](screenshots/new_post_new.png)

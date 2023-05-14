# Quasagram

## Install app dependencies
```bash
npm install
```

## Install backend dependencies
```bash
cd backend
npm install
```

## Add your Heroku project name
- On line 8 of `/backend/package.json` add your own Heroku project name 
```
{
  ...
  "scripts": {
    ...
    "deploy": "heroku builds:create -a [YOUR HEROKU PROJECT NAME]"
  },
  ...
}
```

## Add your own **serviceAccountKey.json** file
- Ensure you have a Firebase Project named Quasagram
- On the Firebase website, on the Project Overview page, add a new web app (if you've not already added one).
- Once created, click on **1 App** > **Cog icon** > **Service accounts**.
- Generate a new private key, store it in your `/backend` folder
- Rename the private key to `serviceAccountKey.json`

## Start the backend (from /backend folder)
```bash
npm start
```

## Start the app in development mode (from / folder)
```bash
quasar dev
```
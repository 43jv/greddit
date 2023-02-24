# Greddit
Greddit is a fully-featured social media web application, built with the MERN stack.  

Deployed at:

## Features
- Create, read, update and delete posts
- Like and unlike posts
- Create, reply to, read, update and delete nested comments
- Markdown for posts and comments
- Sign up and login using JWT for authentication
- Private message users in real-time using socket.io
- View profiles of users and browse through their posts, liked posts and comments
- Infinite scrolling 
- Sort posts by attributes such as like count, comment count and date created
- Profanity filtering and posting/commenting cooldowns
- Update bio which can be viewed by other users
- Search for posts by their title
- Fully responsive layout

## Installation and usage
### Using Docker
1) In root directory run 
   ```
   docker-compose up
   ```
   Use sudo if permissions denied error.

2) To stop the application, run
     ```
    docker-compose down
    ```
### Using npm
1) Install dependencies  
```
cd backend
npm install
cd ..
cd frontend
npm install
```
2) Create .env in backend directory if not already present.
```
cd backend
touch .env
```
3) Configure environment variables in your new .env file. To acquire your MONGO_URI, create a cluster at https://www.mongodb.com/. The TOKEN_KEY is a secret key of your choosing, you can generate one at this site: https://randomkeygen.com/.
```
MONGO_URI=<YOUR_MONGO_URI> 
TOKEN_KEY=<YOUR_TOKEN_KEY>
PORT=4000
```
4) Run the server
```
cd backend
npm start
```
5) Start a new terminal in the root directory and run react's development server
```
cd frontend
npm start
```

# simple-node-app - developing with Docker


This node app shows a simple user profile app set up using 
- index.html with pure js and css styles
- nodejs backend with express module
- mongodb for data storage


All components are docker-based

### With Docker

#### To start the application

Step 1: build the custom image locally

    docker build -t node-app:1.0 .

Step 2: start up the application in detached mode

    docker-compose -f docker-compose.yaml up -d

Step 3: open mongo-express from browser

    http://localhost:8081

Step 4: create `user-account` _db_ and `users` _collection_ in mongo-express

Step 5: Access you nodejs application UI from browser

    http://localhost:3000

Step 6: Shut down the application

    docker-compose down --volume

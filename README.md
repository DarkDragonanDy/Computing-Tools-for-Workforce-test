This repository contains a small Python web application used to practice Git, GitHub, and Docker workflows.

## Application

The application listens on port 8000 and returns a text response when accessed over HTTP.

## Verification

Verify the running application with: curl http://localhost:8080 (host port 8080 maps to container port 8000).
A successful response includes the line: Status: healthy - <NetID>
# Usage

     Build the image:

         docker build -t git-docker-app:test .

     Run the container:

         docker run -d --name app-test -p 8080:8000 git-docker-app:test

     Stop and remove the container:

         docker stop app-test
         docker rm app-test



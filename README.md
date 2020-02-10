# Simple web app for Pluralsight courses and Docker Deep Dive book
This is a quick and dirty node.js app cobbled together for the purposes of demonstrating how to Dockerize/containerize a simple app.

**This app is not maintained and WILL be full of vulnerbilities. Use at own risk**

Exposes web server on port 8080 as per ./app.js

See **Dockerfile** for more details

# My updates
* `npm audit fix`

# Stages of containerized app
1. Build the image `docker image build -t danlavrushko/psweb:1 .`
1. Push to the registry `docker image push danlavrushko/psweb:1`
1. Run the container `docker container run -d --name web -p 8000:8080 danlavrushko/psweb:1`

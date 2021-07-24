
# CI to Docker Hub

A GitHub Action that builds the image defined by the Dockerfile 
and pushes it to Docker Hub 
may be found at `.github/workflows/main.yml`. 

The logs associated with running the workflow may be found under the "Actions" tab in the GitHub repo. 

Once the workflow has executed successfully, one may then run the built image in a Docker Container via: `docker run -p80:80 petermchale/docker-ci`

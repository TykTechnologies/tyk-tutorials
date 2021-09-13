Now that the Docker repo is cloned, we can use a single Docker Compose command to deploy and configure both Redis (prerequisite, needed for token storage and distributed rate limiting) and the Tyk Gateway.  

*  Deploy Tyk Gateway and Redis  
`docker-compose up -d`{{execute}}

You should see these appearing successfully as 'done'  
![Successful deployment](./assets/successful_deployment.png)

*  We can now test the deployment against the 'hello' endpoint  
`curl localhost:8080/hello`{{execute}}

Where we will see a 'pass' status along with the version and some further information.  

Whilst doing Imran Teli's course on Devops, we began to dive into Docker and containerization. Throughout the course, we worked on moving this multi-tier architecture from VM, to [AWS Cloud](https://github.com/andreapeterson/AWS-MultiTier-Architecture), then [reconstructing it in AWS Cloud](https://github.com/andreapeterson/AWS-Webapp-Beanstalk) to include more PaaS and SaaS services, and now finally containerizing it and running it on docker containers.

Following the same schema as the other projects, I customized the webpage once again to feature my sweet pup on the login page. Once again, most of the files comes from [here](https://github.com/devopshydclub/vprofile-project/blob/docker/compose/docker-compose.yml). I customized some of the web files and created the Docker-files & compsoe file for this project.

First, I found the base images on Dockerhub. Nginx, MySQL, and Tomcat needed customization, so they have their own docker files and I created an image out of them on my [Dockerhub Account](https://hub.docker.com/u/andreapeterson).
Then, I created the docker compose file and customized the application.properties file for the application to communicate properly.
Finally, I tested it on EC2 and made changes to fix bugs and once it was perfect, I pushed it the 3 custom containers to Dockerhub. Below is a picture of the final result.

<img width="1645" alt="Screenshot 2024-01-31 at 4 36 55 PM" src="https://github.com/andreapeterson/docker_milowilo/assets/134665743/617e7ae7-a97a-4302-acf0-b846a79376e5">

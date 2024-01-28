# DevOps-Assignment-2
DevOps-Assignment-2

 - Create a new Docker network named "my_network" using the bridge driver
    - docker network create --driver=bridge my_network
 - Create a new Docker container using the "nginx" image and connect it to the "my_network" network. Name the container "nginx_container".
    - docker pull nginx
    - docker run --name nginx_container --network my_network -d nginx
 - Create a new Docker container using the "httpd" image and connect it to the "my_network" network. Name the container "httpd_container".
    -   docker pull httpd
    -   docker run --name httpd_container --network my_network -d httpd
 -  Use the "docker network inspect" command to display information about the "my_network" network. Document your findings in the README.md file.
    - docker network inspect my_network > README.md

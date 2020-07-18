# nginx_k82_https

Repository for the implementation of a 5-replica nginx server on a kubernetes cluster accessible through https.  
The project is organized in the same way as https://github.com/matteobolner/nginx_swarm_https  
The kubernetes cluster is build through k3s (https://k3s.io/)and instantiated on three Ubuntu virtual machines hosted on Amazon Web Services.  
The SSL certificates are encrypted with kubernetes Secrets, and the configuration files managed with kubernetes ConfigMaps

What works:
-The cluster was built succesfully, and can be accessed through https from each of the machines public IP addresses
TODO:
-implement a load balancer

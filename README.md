# keycloak-spike

This is a simple example of keyloak authentication using docker compose, tested using docker machine. 

To test locally, you need the app to be running on your local machine on port 9000. 

You'll need to update the IP address to be the ip of your docker VMhttps://github.com/bnppl/keycloak-spike/blob/master/data/config.yml#L5 (hard coded to 192.168.99.100 in this file in a few locations)

You'll need to update the nginx config to point to your local machine's ip relative to the docker VM in this file
https://github.com/bnppl/keycloak-spike/blob/master/mysite.template#L6 (hard coded to 10.0.2.2) in two locations here.

There is a simple php script to handle redirection that you need to run locally on port 9011.

    php -S localhost:9011 redirect.php


##See also:

https://github.com/gambol99/keycloak-proxy

# SAML Example
A basic SAML setup based on a Keycloak IDP.

## Start the Keycloak IDP (+ postgres db)
> docker-compose up 

## To login to the Keycloak admin console
[Administration Console](http://localhost:9191/auth/admin/)
Login using admin/admin

## Start the ReactJS app
This frontend/saml-enabled-client is an example client (basically a copy from [User Authentication with Keycloak](https://blog.scalac.io/user-authentication-with-keycloak-part1.html)).

> yarn install
> yarn start 

Access the [secure page](http://localhost:3000/secured) (will redirect to IDP for SAML authentication).
Login using barium/barium

## Aditional info
The client side can be configured via 
- public/keycloak.json

Furthermore, SAML metadata files are exported from Keycloak
- ./idp-metadata.xml
- ./sp-metadata.xml can 



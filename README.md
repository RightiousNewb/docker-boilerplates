This repo contains example configurations for setting up a web application via docker containers behind a Traefik v3, and includes Crowdsec for proactive threat prevention. It also includes a basic configuration for DIUN, an application for receiving notifications when new images are available for containers.

In this specific example the application in question is a vtt application called foundryVTT, but any dockerized application could be used in place of this container. 

An external docker network named 'proxy' is required to be created before starting the containers, and crowdsec requires a bit of extra configuration (see .example-acquis.yaml for more).

These boilerplates will require some configuration changes for user IDs, group IDs and sensitive data. They are meant to be a starting point, and not necesarily the final destination / configuration.

Once crowdsec is configured and the proxy network is created, running you can start the containers with docker compose from the root directory to start all of the containers in this project.

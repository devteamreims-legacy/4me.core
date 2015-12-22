# What is 4ME ?

4ME is modular set of tools built to bring non critical operational data to air traffic controlers. 4me's architecture is entirely modular : a set of specialized microservices exchange data via a message queue and/or REST API in order to present relevant operational data to ATCs

# 4me.core

This repo is a placeholder repo for all 4ME.core bricks.

Here's a short description of all :
* 4me.core.ui : Basic interface framework, modular, built with AngularJS and Angular Material
* 4me.core.mq : AMQP message queue, contains configuration files for our broker
* 4me.core.mapping : NodeJS microservice responsible of gathering and maintaining a CWP <-> open sector map, REST API + 4me.core.mq events
* 4me.core.mapping.ui-plugin : Supervisor UI plugin to manage our control room map
* 4me.core.docs : Documentation, build instructions, maintenance.

## Dependencies

Multiple dependancies are required to build and run this set of tools :
* NodeJS
* NPM
* Bower
* Gulp task runner
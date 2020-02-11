# Delivery
Building continuous delivery app on GCP using Flask 

In real business cases while developing and building predictive models are significant part of modern data scientist, it is also crucial to point out how running continious delivery of the model or any project on the fly. One of the amazing python libraries Flask enables that in much faster and effective way. In this quick guide, we try to build simple demo Hello World app and use Flask to add continious delivery of that app using GCP environment. this is the link of the APP: https://deliveryflask.appspot.com

## First of all we set up new project on GCP and follow instructions to build up our Flask Delivery app

![](https://github.com/Ibrokhimsadikov/Delivery/blob/master/Setup_project.JPG)

## After we want to connect our GCP cloud shell with our public github account. We add ssh-keys if not already added to Github: i.e. ssh-keygen -t rsa than upload key to Github ssh settings.

![](https://github.com/Ibrokhimsadikov/Delivery/blob/master/activating%20cloud-shell%20and%20setting%20ssh.JPG)

## We start building our flask application and start developing its attribute file.  We  need the following files which you can create with the following commands. We name them as per instruction given in sample github repo: app.yaml, main.py, main_test.py and requirements.txt from this repo from google. 

Makefile- This allows an easy to remember convention.
App.yaml- This is part of the IaC (Infrastructure as Code) and configures the PaaS environment for Google App Engine.
main.py-  This the logic of the Flask application.
main_test.py- testing application logic
requirements.txt-These are the packages we use.
cloudbuild.yaml- configuration, of flask application for Automating App Engine deployments with Cloud Build

![](https://github.com/Ibrokhimsadikov/Delivery/blob/master/make%20install.JPG)


![](https://github.com/Ibrokhimsadikov/Delivery/blob/master/deploy%20app.JPG)

![](https://github.com/Ibrokhimsadikov/Delivery/blob/master/hello%20world.JPG)

![](https://github.com/Ibrokhimsadikov/Delivery/blob/master/creating%20push%20trigger.JPG)




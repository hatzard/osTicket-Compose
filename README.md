# osTicket-Compose


Greetings!

I created this so you can use osTicket System with Docker!

I have created this composed with the following versions (up to date by the time of creation):


- MySQL: 5.5.62 (min required)
- OSTicket: 1.17.3 (latest version available at this time)
- PHP Version 8.0 Apache (min required for this version as well)


# Usage

The given yml file has all the basic info for having this running. Keep in mind this file was meant to be only for test environment and not for Production. Changes needs to be make to make it worthy for Prod. 

# Final Comments

- I create this DC that uses a Dockerfile to create the image for the Osticket system since OSTicket stopped to give support directly to their Dockerhub with the latest version. After a while, the latest version of the software that I used will be outdated, however, in the Dockerfile you just need to change the download link accordingly to the latest version and the PHP if required. 

- I also let the line commented in case you want to create you own custom image and upload it to your own Dockerhub.


- Again, having plane environment variables with credentials in a docker compose is unrecommended, I made this for testing purposes, you will need to create and point to your own .env file if you want to be a bit secure.

- I created the two folders so they can replicate what you have inside the containers in case you need to make some changes. During the installation process, the system will ask you to make some changes to the upload folder inside /var/log/html so this is an easy way to have access to that directory.








I hope that this become of help to anyone who needs it!



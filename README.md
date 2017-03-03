# Wordpres Development with Docker

This is a base or tempplate for **WordPress development** with **Docker environment** and **folder volumes**. This way you can develop themes, plugins... or even setup a full WordPress site locally without need to install or configure practically anything but Docker.

The main advantage of this configuration is that **you can sync the folder with some sync app/service** (like Dropbox, Google Drive, OneDrive...) and you can continue developing in other computer **without loosing database data**, files or configurations.



This configuration uses [**MySQL** *(latest)*](https://hub.docker.com/_/mysql/) image and [**WordPress** *(latest)*](https://hub.docker.com/_/wordpress/) image **from Docker Hub** and uses local folder volumes to store DB (``./mysqldb``) and WordPress (``./wordpress``) files.

## Usage
1. Clone this repository
2. Install Docker and Docker Composer
3. Use ``docker-compose up`` to begin to develop!

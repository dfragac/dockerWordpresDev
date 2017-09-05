# Wordpres Development with Docker

This is a base or tempplate for **WordPress development** with **Docker environment** and **folder volumes**. This way you can develop themes, plugins... or even setup a full WordPress site locally without need to install or configure practically anything but Docker.

The main advantage of this configuration is that **you can sync the folder with some sync app/service** (like Dropbox, Google Drive, OneDrive...) and you can continue developing in other computer **without loosing database data**, files or configurations.

This configuration uses [**MySQL** *(5.5)*](https://hub.docker.com/_/mysql/) docker image as database server. It also uses [**WordPress** *(php7.1)*](https://hub.docker.com/_/wordpress/) image as base to build a new one with PHPZip library needed for some plugins. This choices are because I use to develop with this server configuration.

This uses local folder volumes to store DB (``./mysqldb``) and WordPress (``./wordpress``) files.

## Usage

For each web you want to develop (You need Docker and Docker Composer installed on your machine):

1. Clone this repository: ``git clone https://github.com/dfragac/dockerWordpresDev.git myweb.com``.
2. Use ``docker-compose up`` on just created folder ``myweb.com``.
3. Access to [http://localhost:8080/](http://localhost:8080/) on your favourite browser.
4. Begin to develop!
# Linux Server Configuration
This is a baseline installation of a Linux server that has been prepared to host a web application.

## IP address and SSH port number
IP address: 18.188.155.200  
SSH port number: 2200

## Complete URL to the hosted web application
http://18.188.155.200.xip.io

## Software installed
In order to properly configure the server to host the catalog-app web application, the following packages were installed:  
`apache2`
`libapache2-mod-wsgi-py3`
`postgresql`
`python3-pip`  

From the Python Package Index, the following were installed:  
`flask`
`SQLAlchemy`
`psycopg2`

## Configurations made
1. The timezone was configured to UTC using `sudo dpkg-reconfigure tzdata`.
2. A UFW firewall was configured and activated, disaabling all incoming ports except for `SSH` 2200, `HTTP` 80, and `NTP` 123.
3. An Apache2 web server was configured.
4. A PostgreSQL database was configured. In addition, a user with limited permissions for the hosted web application was added through the `createuser` command and answering the following:  
`Shall the new role be a superuser? (y/n) n`  
`Shall the new role be allowed to create databases? (y/n) y`  
`Shall the new role be allowed to create more new roles? (y/n) y`  

## List of third-party resources used
Several sites helped in understanding how to properly configure and setup the server, as well as correctly hosting the application. Among those included DigitalOcean, Udacity, and Stack Overflow. One particularly helpful resource was [this tutorial by Manuel](https://www.youtube.com/watch?v=3HuYr6G2Z28&t=1093s).

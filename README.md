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
1. The timezone was configured to UTC.
2. A UFW firewall was configured and activated.
3. Apache2 web server was configured.
4. PostgreSQL database was configured and a user with limited permissions for catalog application was added.

## List of third-party resources used
Several sites helped in understanding how to properly configure and setup the server, as well as correctly hosting the application. Among those include DigitalOcean, Udacity, and Stack Overflow. One particularly helpful resource was [this tutorial by Manuel](https://www.youtube.com/watch?v=3HuYr6G2Z28&t=1093s).

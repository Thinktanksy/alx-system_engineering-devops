0x0C. Web server

In this project, we will be exploring the concepts and components of a web server. We will learn how to set up a basic web server, configure virtual hosts, handle DNS resolution, and understand different HTTP headers and status codes.



Table of Contents

    Requirements
    Installation
    Usage
    Configuration
    Testing
    Resources

Requirements

    Ubuntu 18.04 LTS
    Nginx

Installation

To install Nginx, follow these steps:

    Open a terminal.
    Update the package index by running the following command:
sudo apt update

Install Nginx by running the following command:


sudo apt install nginx

Usage

To start the Nginx web server, use the following command:

sudo service nginx start
Once the server is running, you can access it by opening a web browser and navigating to http://localhost.

To stop the Nginx server, use the following command:


sudo service nginx stop

Configuration

The main configuration file for Nginx is located at /etc/nginx/nginx.conf. You can edit this file to modify the server's settings, such as the number of worker processes, log file locations, etc. It's important to understand the Nginx configuration directives and their meanings before making any changes.

In addition to the main configuration file, Nginx also uses configuration files located in the /etc/nginx/sites-available/ directory for setting up virtual hosts. You can create separate configuration files for different websites and enable them by creating symbolic links in the /etc/nginx/sites-enabled/ directory.
Testing

To test the Nginx configuration for syntax errors, use the following command:

bash

sudo nginx -t

If there are no errors, you will see a success message. Otherwise, it will display the specific error(s) that need to be fixed.
Resources

    Nginx Official Documentation

# Web Application Deployment Project

##Overview

This project is basically about setting up a static web application and getting it running on Ubuntu Linux. I used both Nginx and Apache for the web servers, since the assignment in
DevOps training wanted that kind of setup. Nginx handles the main traffic on port 80, and Apache is on 8080 to keep things from clashing.

## Technologies Used
- Nginx - Primary web server running on port 80

- Apache2 - Secondary web server running on port 8080

- Git - Version control for all configuration and application files

- Ubuntu 16.04 LTS - Host operating system

## Deployment Notes
Nginx is configured as the primary web server serving webapp.local on port 80 with a custom 404 error page and separate access and error logs.


Apache is configured on port 8080 to avoid conflict with Nginx. A .htaccess file handles URL redirection using mod_rewrite, redirecting /home to the root path with a 301 permanent redirect.
Both servers serve the same static HTML files from separate directories.All configuration files are version controlled using Git with a feature branch workflow,
ensuring clean commit history and easy rollback.

##Author
Aayush Shrestha - DevOps Training Week 2 Assignment

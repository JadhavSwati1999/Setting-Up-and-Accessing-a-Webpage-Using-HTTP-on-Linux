# Setup & Access Webpage.

In this project I have used Web Server HTTPD service, how we can set up a web server in our Linux environment, deploy our first simple HTML-based web page, and how we can access our web page from a browser.

## What is HTTPD ?

HTTP Daemon is a software program that runs in the background of a web server and waits for incoming server requests.

The daemon answers the request automatically and serves the hypertext and multimedia documents over the Internet using HTTP.

Launch an EC2 instance and connect it to CLI

- Install httpd service.

yum install httpd



- Check the status of the httpd service

systemctl status httpd.service



- Start the service

systemctl start httpd.service


- Create the html file under /var/www

cd /var/www ——>ls—→cd html

- Create a html file

vi index.html



- Simple HTML code is written inside the index.html



- Copied the image from the local machine to the remote machine

scp -i “key” source path username@destination_path


- Moved the image from home directory to the html directory


- The website is successfully hoisted using the public IP of the instance.


# Summary

Successfully hosted website using httpd service through AWS EC2 instance CLI

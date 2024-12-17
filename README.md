# AltSchool Project
This project is to demonstrate my ability in hosting a web application. This application is hosted on AWS Cloud, using nginx as the webserver and Ansible for server configuration, Let's Encrypt for SSL Certificate and Certbot for automatic renewal of the SSL certificate.


# Architecture
![Architecture](./media/Cloud%20Architecture.jpeg)


# GitHub Structure

- Website
    - Directory contains HTML and CSS
- Playbook
    - Directory contains Ansible configuration files.
- Media
    - Directory contains media files.


# Step by Step guide

- Provisioned an Ec2 instance running Ubuntu on AWS 
    - Configured security group for SSH on port 22, HTTP on port 80 and HTTPS on port 443 
- write HTML and CSS for the landing page
- DNS resolution
    - Register a domain name (oyameogbeche.cloud)
    - created hosted zones in Route53
    - configured NS records
    - created A record for subdomain (altschool.oyameogbeche.cloud)
- Setup Ansible control node
    - establish ssh connection from the control node to the managed node
    - write ansible play files to install, enable nginx and deploy website files
    - write ansible play to configure SSL encrption and auto renewal of SSL certificate with certbot and Let's Encrypt


# URL
https://altschool.oyameogbeche.cloud


# Contact 
If you have any questions or suggestions, please feel free to open an issue or contact me by [email](mailto:oyogbeche@gmail.com) or [LinkedIn](https://www.linkedin.com/in/oyameogbeche/)
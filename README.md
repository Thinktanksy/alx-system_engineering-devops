0x0F Load Balancer

This project focuses on implementing a simple HTTP load balancer using Nginx. The load balancer distributes incoming web traffic across multiple backend servers to improve scalability, reliability, and performance.
Description

The load balancer project consists of configuring Nginx to distribute HTTP requests among two web servers. The load balancer acts as an intermediary between the client and the backend servers, ensuring that the traffic is evenly distributed across the available servers.

The project involves the following tasks:

    Configuring two web servers: web-01 and web-02, both running on Ubuntu.
    Installing and configuring Nginx on a separate server.
    Configuring Nginx to balance the HTTP traffic between web-01 and web-02.
    Adding a custom Nginx response header to identify which server is handling the request.

Files

The following files are part of this project:

    README.md: Provides an overview and instructions for the project.
    0-custom_http_response_header: Bash script to configure Nginx with a custom response header.
    1-install_load_balancer: Bash script to install and configure Nginx as a load balancer.
    2-puppet_custom_http_response_header.pp: Puppet manifest to configure Nginx with a custom response header using Puppet.
    3-puppet_install_load_balancer.pp: Puppet manifest to install and configure Nginx as a load balancer using Puppet.
Getting Started

To use the load balancer and configure Nginx, follow these steps:

    Start by cloning this repository to your local machine:
    Review the contents of each file to understand the configuration and installation steps involved.

    Ensure you have access to the required servers: web-01, web-02, and the load balancer server.

    Execute the scripts or manifests on the respective servers according to your preferred method:

        Bash scripts:
            0-custom_http_response_header on web-01 and web-02 to configure the custom response header.
            1-install_load_balancer on the load balancer server to install and configure Nginx as a load balancer.

        Puppet manifests:
            2-puppet_custom_http_response_header.pp on web-01 and web-02 to configure the custom response header.
            3-puppet_install_load_balancer.pp on the load balancer server to install and configure Nginx as a load balancer.

    Verify the load balancer configuration by making HTTP requests to the load balancer server and checking that the traffic is distributed among the backend servers.

Resources

    Introduction to Load Balancing
    HTTP Load Balancing with Nginx

Author

This project was created by [Your Name].

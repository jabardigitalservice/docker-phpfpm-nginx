# Docker PHP-FPM & Nginx on Alpine Linux

Example PHP-FPM & Nginx setup for Docker, build on [Alpine Linux](http://www.alpinelinux.org/).
The image is only +/- 35MB large.

* Built on the lightweight and secure Alpine Linux distribution
* Very small Docker image size (+/-35MB)
* Uses latest PHP version for better performance, lower CPU usage & memory footprint
* Optimized for 100 concurrent requests (optimized for container with limit 0.25 vcpu, 512 mb)
* Optimized for building micro RESTful API
* The servers Nginx, PHP-FPM and supervisord run under a non-privileged user (nobody) to make it more secure
* The logs of all the services are redirected to the output of the Docker container (visible with `docker logs -f <container name>`)
* Follows the KISS principle (Keep It Simple, Stupid) to make it easy to understand and adjust the image to your needs

## Credits
Forked from https://github.com/TrafeX/docker-php-nginx
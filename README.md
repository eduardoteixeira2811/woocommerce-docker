# woocommerce-docker
A container that provides Wordpress, WooCommerce and the Wirecard extension with all versions

# Usage
1. Edit the variables in .env to your needs
Use the versions numbers from the following sources:
Wordpress: https://hub.docker.com/_/wordpress?tab=tags (use the tag name that contains the PHP and wordpress version of your choice)
WooCommerce: https://wordpress.org/plugins/woocommerce/advanced/ (scroll down to the versions dropdown)
Wirecard WooCommerce extension: https://wordpress.org/plugins/wirecard-woocommerce-extension/advanced/ (scroll down to the versions dropdown)
2. Run ```docker-compose up```

If you are done, stop the container with ```docker-compose down --volume``` 

# Example Use Cases
## Run latest WooCommerce with latest Wordpress, latest WD extension and PHP 7.3
Change the following variables in .env file:
WORDPRESS_VERSION=latest
WOOCOMMERCE_VERSION=4.3.1
WIRECARD_VERSION=3.3.4

## Run WooCommerce beta with latest Wordpress, latest WD extension and PHP 7.3
Change the following variables in .env file:
WORDPRESS_VERSION=5.5.0-php7.3
WOOCOMMERCE_VERSION=4.4.0-beta.1
WIRECARD_VERSION=3.3.4


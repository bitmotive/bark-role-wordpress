# BARK: WordPress

## Description
Install and configure WordPress on a server with MySQL and Nginx.

## Requirements
All roles in the Bitmotive Ansible Role Kit are configuration driven.
Customize this role by providing environment variables in either your
shell environment, host specific in group_vars/, or at the CLI when
prompted at runtime. 

## Role Variables

**WORDPRESS_MYSQL_ROOT_PASSWORD**:

The root password for the MySQL database used by WordPress.

**WORDPRESS_DB_NAME**:

The name of the WordPress database.

**WORDPRESS_DB_USER**:

The username for the WordPress database user.

**WORDPRESS_DB_USER_PASSWORD**:

The password for the WordPress database user.

**WORDPRESS_SERVER_ROOT**:

The root directory where WordPress files will be stored on the server.

**WORDPRESS_NGINX_HOSTNAME**:

The hostname for the Nginx server.

**WORDPRESS_NGINX_PORT**:

The port number on which Nginx will listen for WordPress traffic.

**WORDPRESS_NGINX_SSL_ON**:

Whether SSL should be enabled for the Nginx server (YES/NO).

**WORDPRESS_NGINX_PUBKEY**:

The path to the SSL public key file for Nginx.

**WORDPRESS_NGINX_PRIVKEY**:

The path to the SSL private key file for Nginx.

**WORDPRESS_REDIRECT_WWW**:

Whether to redirect www subdomain to non-www domain or vice versa (YES/NO).

## Dependencies
- Ubuntu
- MySQL/MariaDB
- Nginx
- PHP and required extensions

## Functionality
- Sets up WordPress with the specified database credentials
- Configures Nginx as the web server
- Enables SSL if specified
- Sets up WWW redirection if specified

## License
MIT

## Author Information
A Bitmotive Project: Build. Incubate. Train.
https://bitmotive.com

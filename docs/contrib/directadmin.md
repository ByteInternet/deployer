<!-- DO NOT EDIT THIS FILE! -->
<!-- Instead edit contrib/directadmin.php -->
<!-- Then run bin/docgen -->

# Directadmin Recipe

```php
require 'contrib/directadmin.php';
```

[Source](/contrib/directadmin.php)



### Configuration
- `directadmin` – array with configuration for DirectAdmin
    - `host` – DirectAdmin host
    - `port` – DirectAdmin port (default: 2222, not required)
    - `scheme` – DirectAdmin scheme (default: http, not required)
    - `username` – DirectAdmin username
    - `password` – DirectAdmin password (it is recommended to use login keys!)
    - `db_user` – Database username (required when using directadmin:createdb or directadmin:deletedb)
    - `db_name` – Database namse (required when using directadmin:createdb)
    - `db_password` – Database password (required when using directadmin:createdb)
    - `domain_name` – Domain to create, delete or edit (required when using directadmin:createdomain, directadmin:deletedomain, directadmin:symlink-private-html or directadmin:php-version)
    - `domain_ssl` – Enable SSL, options: ON/OFF, default: ON (optional when using directadmin:createdb)
    - `domain_cgi` – Enable CGI, options: ON/OFF, default: ON (optional when using directadmin:createdb)
    - `domain_php` – Enable PHP, options: ON/OFF, default: ON (optional when using directadmin:createdb)
    - `domain_php_version` – Domain PHP Version, default: 1 (required when using directadmin:php-version)



## Tasks

### directadmin\:createdb {#directadmin-createdb}
[Source](https://github.com/deployphp/deployer/blob/master/contrib/directadmin.php#L76)

Creates a database on DirectAdmin.




### directadmin\:deletedb {#directadmin-deletedb}
[Source](https://github.com/deployphp/deployer/blob/master/contrib/directadmin.php#L96)

Deletes a database on DirectAdmin.




### directadmin\:createdomain {#directadmin-createdomain}
[Source](https://github.com/deployphp/deployer/blob/master/contrib/directadmin.php#L111)

Creates a domain on DirectAdmin.




### directadmin\:deletedomain {#directadmin-deletedomain}
[Source](https://github.com/deployphp/deployer/blob/master/contrib/directadmin.php#L129)

Deletes a domain on DirectAdmin.




### directadmin\:symlink-private-html {#directadmin-symlink-private-html}
[Source](https://github.com/deployphp/deployer/blob/master/contrib/directadmin.php#L145)

Symlink your private_html to public_html.




### directadmin\:php-version {#directadmin-php-version}
[Source](https://github.com/deployphp/deployer/blob/master/contrib/directadmin.php#L161)

Changes the PHP version from a domain.





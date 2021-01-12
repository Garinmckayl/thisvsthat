# Servers

Table of Contents
=================

   * [Apache vs Nginx](#Apache-vs-Nginx)



## Apache vs Nginx

## Apache
Apache also know as httpd is a http server that powers 46% of the web.
Apache allows configuration via .htaccess file, this access is external per-directory configuration. 
Apache .htaccess Example for redirecting.

```apache
RedirectMatch 301 ^/blog /blog.html
```

## Nginx
Nginx pronounced Engine x. 
Nginx is an extremely performant server, It Can handle more than 10000 simultaneous connections. 

It is Commonly used as a reverse proxy(distribute the load to multiple backend servers), like database servers, application server. 
Nginx does not allow external configuration like apache(htaccess).
Configuration file can be found on etc directory. 

```
File: /etc/nginx/nginx.conf
```
Here is extremely simple nginx,conf file.

```nginx
worker_processes 1;
daemon off;
error_log nginx_error.log;
events {
    worker_connections 1024;
}

http {
    server {
        listen 8008;

        location / {
            root /Users/bsergean/src/sandbox/json/jsoncpp;
        }
    }
}
```

Defining directives allows you to customize Nginx.  
If a directive is followed by braces it is called context, and a context can contain more directives. [More info about nginx conf can be found here](http://nginx.org/en/docs/beginners_guide.html).
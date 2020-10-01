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
Nginx does not allow external configuration like apache(htaccess) 
Try following nginx config.

```nginx
server {
  listen 80;
  server_name  your.domain.com;

  location / {
    alias /path/to/dir/of/docs/;
    index index.html;
  }
}
```
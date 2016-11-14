# nginx_learning

install from brew: $brew install/uninstall nginx.

start/stop: $sudo sudo nginx/ -s stop.

brew need user has ownership on /usr/local, so need $sudo chown -R `whoami` /usr/local.

nginx html folder (brew install only) is by the defult in:
  /usr/local/Cellar/nginx/nginx_version/html.

location setting:

location / {
            root   /where/index/folder;
            index  index.html index.htm;
        }

        location /images/ {
            root   /where/images/folder;
            
        }

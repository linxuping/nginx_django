nginx:
sudo /usr/sbin/nginx -t -c /etc/nginx/nginx.conf --fortest
sudo /usr/sbin/nginx -c /etc/nginx/nginx.conf
sudo /usr/sbin/nginx -s reload   --valid config

django:
python manage.py runfcgi method=prefork host=127.0.0.1 port=9001

refer to:
Django项目在nginx上面的部署(django+flup+nginx) http://www.linuxyan.com/shell/249.html



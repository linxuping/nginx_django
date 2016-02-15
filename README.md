nginx:
sudo /usr/sbin/nginx -t -c /etc/nginx/nginx.conf --fortest
sudo /usr/sbin/nginx -c /etc/nginx/nginx.conf
sudo /usr/sbin/nginx -s reload   --valid config

django:
python manage.py runfcgi method=prefork host=127.0.0.1 port=9001

refer to:
Django项目在nginx上面的部署(django+flup+nginx) http://www.linuxyan.com/shell/249.html
windows下安装设置Nginx+python+flup+django,并设为服务运行 http://blog.sina.com.cn/s/blog_3cb6a78c0100r677.html

visit:
http://192.168.10.102:8080/index


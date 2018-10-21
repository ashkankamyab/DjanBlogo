## Deployment Documentation

[Reference #1](https://www.digitalocean.com/community/tutorials/how-to-serve-django-applications-with-uwsgi-and-nginx-on-ubuntu-16-04)
[Reference #2](https://docs.nginx.com/nginx/admin-guide/web-server/app-gateway-uwsgi-django/)
[Reference #3 ](https://uwsgi-docs.readthedocs.io/en/latest/WSGIquickstart.html)

There is different Methods to deply Django using uwsgi, but unfortunatly there is no Pestpractice for it.
I have had tried different Method as well and here is first which worked pretty well. May some one help to
contribute it and define the Best Practice, Pull Requests always are welcome.


### Setup uwsgi
Make sure all dependencies are installed
``` sh
sudo apt install python3-pip python3-dev
```
Preferably install uwsgi using PyPip. I am using virtualen using virtualenvWrapper.
Upgrage pip using pip
``` sh
sudo -H pip3 install --upgrade pip
sudo -H pip3 install virtualenv virtualenvwrapper
```
We should define python3 full-path for Virtualenvwrapper to work properly
I set working directory \'Env\' regarding to Reference \#1 you can to determin whatever you like.


``` sh
echo "export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3" >> ~/.bashrc
echo "export WORKON_HOME=~/Env" >> ~/.bashrc
echo "source /usr/local/bin/virtualenvwrapper.sh" >> ~/.bashrc
```
we may could source the ".bashrc' file then.
``` sh
source ~/.bashrc
```

So is so far, right?
- [ ] Please write the Rest of Document after you are finish with @Jadi

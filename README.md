# KARI_UVINet
Install Guide

### Install dependencies
```
$ curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash -
$ sudo apt-get install -y nodejs
$ node -v
$ sudo npm install -g pm2
$ pm2 install pm2-logrotate
$ pm2 set pm2-logrotate:retain 30
```

### Run Project
```
$ npm install
$ node acm_uvinet.js
```

### Set Autostart
```
$ pm2 start acm_uvinet.js
$ pm2 startup
 >>> sudo env PATH...로 시작하는 경로 전부 입력
$ pm2 save
```

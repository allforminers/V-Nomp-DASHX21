# Node Open Mining Portal
[![Join the chat at https://github.com/blockinator/v-nomp/](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/blockinator/v-nomp?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![Matrix](https://img.shields.io/matrix/v-nomp:matrix.mofumofu.me?label=matrix)](https://app.element.io/#/room/#v-nomp:matrix.mofumofu.me)
[![Build Status](https://travis-ci.com/blockinator/v-nomp.svg?branch=main)](https://travis-ci.org/blockinator/v-nomp)
[![CircleCI](https://circleci.com/gh/blockinator/v-nomp/tree/main.svg?style=svg)](https://circleci.com/gh/blockinator/v-nomp/tree/main)

This is a Yescrypt, YesPower, Lyra2REv2, CPUpower, power2b, YesPowerSugar, sha256d and more algo mining pool based off of Node Open Mining Portal.


#### Requirements
* Coin daemon(s) (find the coin's repo and build latest version from source)
* [Node.js](http://nodejs.org/) v8.11+ ([follow these installation instructions](https://github.com/joyent/node/wiki/Installing-Node.js-via-package-manager))
* [Redis](http://redis.io/) key-value store v2.6+ ([follow these instructions](http://redis.io/topics/quickstart))

##### Seriously
Those are legitimate requirements. If you use old versions of Node.js or Redis that may come with your system package manager then you will have problems. Follow the linked instructions to get the last stable versions.


[**Redis security warning**](http://redis.io/topics/security): be sure firewall access to redis - an easy way is to
include `bind 127.0.0.1` in your `redis.conf` file. Also it's a good idea to learn about and understand software that
you are using - a good place to start with redis is [data persistence](http://redis.io/topics/persistence).


#### 0) Setting up coin daemon
Follow the build/install instructions for your coin daemon. Your coin.conf file should end up looking something like this:
```
rpcuser=hcdcddfghhgfhfgh
rpcpassword=hdfghjjkkjkjkjkj
rpcallowip=127.0.0.1
server=1
rpcport=9998
txindex=1
addresstype=legacy
fallbackfee=0.00001

```


#### 1) Downloading & Installing

Clone the repository and run `npm update` for all the dependencies to be installed:

```bash
sudo apt-get install libminiupnpc-dev libzmq3-dev libprotobuf-dev protobuf-compiler libqrencode-dev unzip software-properties-common redis-server npm git screen -y
sudo apt-get install build-essential libsodium-dev npm libboost-all-dev libgmp-dev redis-server -y
sudo apt install nodejs node-gyp libssl1.0-dev -y
sudo apt install npm -y
sudo npm install n -g
sudo n v12
sudo apt purge nodejs npm -y
sudo ln -sf /usr/local/bin/node /usr/bin/node
sudo ln -sf /usr/local/bin/npm /usr/bin/npm
git clone https://github.com/blockinator/v-nomp
cd v-nomp
npm install
```


````


#### 3) Start the portal

```bash
npm start
```



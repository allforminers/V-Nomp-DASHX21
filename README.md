# Node Open Mining Portal


This is a Yescrypt, YesPower, Lyra2REv2, CPUpower, power2b, YesPowerSugar, sha256d and more algo mining pool based off of Node Open Mining Portal.







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
git clone https://github.com/allforminers/V-Nomp-DASHX21.git vnomp
cd vnomp
npm install
```


````


#### 3) Start the portal

```bash
npm start
```



# Algorand Development Environment

## Algokit Setup
Install pix (https://pipx.pypa.io/stable/)
```
$ sudo apt update
$ sudo apt install pipx
$ pipx ensurepath
```
Restart the terminal window
```
$ pipx install algokit
$ algokit --version
algokit, version 2.5.2
```
Start Docker desktop and then start the algokit local network
```
$ algokit localnet start
```
To use the local blockchain explorer
```
$ algokit explore
```


## npm Setup (for typescript Algorand digital marketplace)
Download nvm (node version manager)
```
$ curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
$ source ~/.bashrc
```

Install the latest stable node release
```
$ nvm install --lts
Installing latest LTS version.
Downloading and installing node v22.13.0...
Downloading https://nodejs.org/dist/v22.13.0/node-v22.13.0-linux-x64.tar.xz...
################################################################################################## 100.0%
Computing checksum with sha256sum
Checksums matched!
Now using node v22.13.0 (npm v10.9.2)
Creating default alias: default -> lts/* (-> v22.13.0)
$ node --version
v22.13.0
$ npm --version
10.9.2
```

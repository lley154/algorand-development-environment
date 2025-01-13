# Algorand Development Environment
https://developer.algorand.org/docs/get-started/algokit/

## Algokit Setup Ubuntu Linux OS
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
$ algokit localnet reset
```

Create a wallet with 2 accounts
```
$ algokit localnet console
# goal wallet new myWallet

# goal account new -w myWallet
Please enter the password for wallet 'myWallet': 
Created new account with address F3YQEH5YNA5MYXOZYNXLJFKZ3H4ZYVCTMJSRNB6AIJSPEMFXRP5Y57WEEM

# goal account new -w myWallet
Please enter the password for wallet 'myWallet': 
Created new account with address CESUDEEE47NDTCDMQM6L6EASLQIHH7GPIVTN37NGFQRXPYKOT2FQ2MHZVQ
```

Launch the local blockchain explorer
```
$ algokit explore
```
- Select the Wallet Connect button on the top right
- Select the myWallet in the wallet dropdown menu
- Select Connect KMD
- Enter the password you set when creating the wallet above
- Fund one of the accounts
- Create a transaction to send funds between the two accounts using the transaction wizard


## npm Setup (for the typescript Algorand marketplace)
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

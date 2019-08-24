#add metamask extension to chrome/firefox :
https://metamask.io/


#install snap for ubuntu :
$ sudo apt install snapd


#install VSCode :
windows/mac : https://code.visualstudio.com/download
ubuntu : $ sudo snap install code --classic


#install sublime:
ubuntu :
$ wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
$ echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
$ sudo apt install sublime-text

windows : https://www.sublimetext.com/3


#install nodejs:

windows : https://nodejs.org/en/download/

mac : brew install node

ubuntu:
$ sudo apt-get install curl
$ curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
$ sudo apt install nodejs
$ node -v
$ npm -v


#install truffle:

windows:
$ npm install -g npm
$ npm install -g ethereumjs-testrpc
$ npm install -g truffle

ubuntu/mac:
$ npm install -g truffle


#run testrpc(windows) :
$ testrpc


#install ganache-cli:

npm : $ npm install -g ganache-cli

yarn : $ yarn global add ganache-cli

install ganache GUI : https://www.trufflesuite.com/ganache


#run ganache:

$ ganache-cli --port 8545

# ERC-20-
This is my repository regarding blockchain.
# Here are the steps to create a ERC 20 token.
1. Create your metamask wallet by adding the extension of metamask to your chrome through this link.
 https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn/related
2. Create token on goerli test network
   chrome-extension://nkbihfbeogaeaoehlefnkodbefgpgknn/home.html#
3. In metamask, go to the setting and connect the metamask to Goerli Test network.
4. You will see that your wallet is  currently empty, so you need to mine it through this link-
   https://goerli-faucet.pk910.de/

#20lab
1. Go to https://20lab.app/ to connect your metamask wallet with 20lab.
2. Choose blockchain Goerli Testnet, then enter your token name,token symbol,initial supply(take a very large number),18 decimals.
3. Choose the desired features then save it.
 https://20lab.app/dashboard/view/0xf07924Ed685ceD1c9115FfD2Ce369bC3A89d98e6
4. Then,Validate and Compile, it will connect to your metamask for GoerliETH(gas fee).
5. Then you can see your Token name (ADM) and address in dashboard.
6. We can see our transaction done on goerli etherscan through this link..
   https://goerli.etherscan.io/tx/0x96371efd3778d7c1966674a1448fbb6b203f350cca37901195c9ce54f934500e
7. We can also check our transactions at metamask etherscan through this link...
   https://goerli.etherscan.io/token/0xf07924Ed685ceD1c9115FfD2Ce369bC3A89d98e6


#Hyperledger-Fabric
To initiate a private blockchain like Hyperledger-Fabric, we need to install docker on our ubuntu system.
For that, We should follow the following codes which we should paste in the terminal to get docker installed..
1.Install Docker
sudo apt-get -y install docker-compose
2. Install Golang-go
sudo apt install golang-go
3. Install jq
(jq is like sed for JSON data )

sudo apt install jq
4. Install Node/java
sudo apt install npm
npm install node
5. Installing Fabric-samples Repository
curl -sSLO https://raw.githubusercontent.com/hyperledger/fabric/main/scripts/install-fabric.sh && chmod +x install-fabric.sh

Then you can pull docker containers by running one of these commands:

./install-fabric.sh docker samples
./install-fabric.sh d s
To install binaries for Fabric samples you can use the command below:

./install-fabric.sh binary
#Building First Network

Navigate through the Fabric-samples folder and then through the Test network folder where you can find script files using these we can run our network.

cd fabric-samples/test-network

We would be running ./network.sh down command to remove any previous network containers or artifacts that still exist.

./network.sh down

we can bring up a network using the following command. This command creates a fabric network that consists of two peer nodes and one ordering node

 ./network.sh up
 
Now our first Hyperledger Fabric Network is successfully running.



 

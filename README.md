MWF- Blockchain Integration 

This project aims at providing a blockchain implementation using Hyperledger Fabric to store the logs generated by MWF(Open-City) Application. Instead of sharing Open Ended Data of MWF in a normal fashion, this solution provides storage of prominance data(logs) in Blockchain which is highly reliable and secure(tamper free).

----------------------------------------------------------------------------------------------------

Steps to run the project application

	1)	To run the application you first need to clone our github repository Command.
		$ git clone https://github.com/Jolig/Blockchain

	2)	To deploy blockchain run the following command.
		$ ./deploy_blockchain.sh

By running the previous command we set the appropriate environment settings and start either a single peer with membership services network or a four peer with membership services network(This will by default start single peer, any other number of peers could be configured).

----------------------------------------------------------------------------------------------------

Leave the network running on one terminal and start the nodejs application on another terminal which would receive requests from  MWF application and send back response. This application could be run by following command -

	3)	start the blockchain application.
		$ node controller.js

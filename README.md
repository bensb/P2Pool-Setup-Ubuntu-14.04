P2Pool-Setup-Ubuntu-14.04
=========================
This guide does not require advanced Linux knowledge.

1. Install Ubuntu Server 14.04 (Digital Ocean is a good provider of VPS)

2. Install Bitcoin
	
	sudo apt-get install python-software-properties
	sudo add-apt-repository ppa:bitcoin/bitcoin 
	sudo apt-get update
	sudo apt-get install bitcoind
	
3. Configuring Bitcoin
	NOTE: Type: "mkdir ~/.bitcoin/" to create this directory.
	
	Edit the file:
		nano ~/.bitcoin/bitcoin.conf
			
			server=1
			daemon=1
			rpcuser=usernamehere
			rpcpassword=SuperSecretPassword
			
4. Starting Bitcoind

	bitcoind
	bitcoind help
	
The blockchain download will begin now, typically takes a day or so to complete.
	
	
	



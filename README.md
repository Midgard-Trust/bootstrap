# securus bootstrap blockchain
What is Bootstrap.dat?
Bootstrap.dat is a file that contains the copy of blockchain from genesis block to a certain point of time. This compressed Bootstrap.dat file is used to speed up the initial blockchain download times. How? Your wallet client downloads and verifies each blocks from the P2P network. This is usually slow and especially if you are using wallet for the first time then syncing process can take quite a long time.

Instead of using Peer to Peer communication your wallet client can read blockchain data from this compressed bootstrap file which contains the copy of blockchain data until a certain block height. Once the wallet client completes reading data from bootstrap file, it will then use the P2P connection to download the remaining blocks. This method is faster and moreover it consumes less bandwidth compared to standard synchronization process. However still bootstrap method takes some time as your wallet client needs to validate each individual blocks.

1. The most recommended step before making any changes to your wallet is taking wallet backup. Have a copy of wallet.dat file in two or more locations. If your wallet is new or empty then this step is not required. Once backup is done exit the wallet.
2. Next you need to move this bootstrap.dat file to your wallet core folder. All cryptocurrency wallet maintains its core files at the following location.


Windows: C:\Users\%username%\AppData\Roaming\Securus

Mac OS: ~/Library/Application Support/securus

Linux: ~/.securus


https://www.securuscoin.org/bootstrap.dat

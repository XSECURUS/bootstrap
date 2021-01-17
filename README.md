# bootstrap
Bitcoin is a Peer to Peer cryptocurrency. The wallet client of Bitcoin downloads blockchain from the network by syncing with other nodes. Not just Bitcoin but most of the cryptocurrency core wallet works like this as they are all based on Bitcoin. Since it requires Peer to Peer communication to download and validate each blocks the process of synchronizing the whole blockchain will be slow. Even computers with high Internet speed will take days or even weeks to sync the Bitcoin blockchain. This is a problem with Bitcoin and other cryptocurrency wallets whose blockchain file size is huge. You can add nodes to your wallet which will help with the network connection but it doesn’t speed up the synchronization process. Fortunately, to accelerate the wallet synchronization process you can use Bootstrap file.

What is Bootstrap file and how it works? Where can I find Bootstrap.dat for Bitcoin and how to use this file?

What is Bootstrap.dat?
Bootstrap.dat is a file that contains the copy of blockchain from genesis block to a certain point of time. This compressed Bootstrap.dat file is used to speed up the initial blockchain download times. How? Your wallet client downloads and verifies each blocks from the P2P network. This is usually slow and especially if you are using wallet for the first time then syncing process can take quite a long time.

Instead of using Peer to Peer communication your wallet client can read blockchain data from this compressed bootstrap file which contains the copy of blockchain data until a certain block height. Once the wallet client completes reading data from bootstrap file, it will then use the P2P connection to download the remaining blocks. This method is faster and moreover it consumes less bandwidth compared to standard synchronization process. However still bootstrap method takes some time as your wallet client needs to validate each individual blocks.

Where can I find this Bootstrap.dat file for Bitcoin?
First of all we’d like to let you know that downloading bootstrap.dat file for Bitcoin from unofficial and untrusted source is highly not recommended. This recommendation is not only for Bitcoin but for other crypto currencies as well such as Dash, Litecoin, etc. You’ll find bootstrap.dat file in torrent, Bitcoin Talk forums and in several third party websites. But as we said these are unofficial sources and they are maintaining it for research purpose. So where can I find the official bootstrap.dat file for Bitcoin?

Bitcoin.org used to provide this bootstrap file to accelerate the synchronization process. But that file is not available and they no longer maintain it. Because syncing wallets using bootstrap.dat method is no longer advantageous and is not necessary anymore. As of Bitcoin Core version 0.10.0 and later downloading blockchain using peer to peer network is much faster and downloading blockchain directly using core wallet client is much efficient.

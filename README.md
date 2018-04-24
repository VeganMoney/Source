
VeganMoney development tree

VeganMoney is a PoS-PoW , Merchant based cryptocurrency.

Development process
===========================

Coin development -- done
PoS Reward System Phase 1 -- done
PoW -- Done
Pre mine for PoS Rewards  -- done
Wallet -- done
Daemon -- done
Linux wallet -- done

To Do;

Roadmap
Whitepaper
Website
Marketplace
Webwallet

Mining Instructions :

Block Reward 100
Block Time    60 seconds
Algorithm Scypt
PoW ends block 10 000
Full PoS Reward system starts at Block 10 001

Pre Mine 2 % .
Pre Mine is to fund development , Exchange listings , fund additional PoS rewards.
25 % of the Pre Mine held by developers to be released in intervals over 12 months.

Open your wallet, and make sure you are connected to another wallet. 
You are connected when you see the icon Wallet Connections in the lower right corner of your wallet.
Close your wallet and create the file veganmoney.conf in the folder "%APPDATA%\veganmoney\".

Paste the following text into veganmoney.conf and save the file.

rpcuser=new username here
rpcpassword=new password
rpcallowip=127.0.0.1
rpcport=36890
listen=1
server=1
addnode=node.walletbuilders.com

Download the latest version of cpuminer from here https://bitcointalk.org/index.php?topic=55038.0 and extract the zip file.

Create a .bat file named mine.bat and paste one of the following text lines into mine.bat.
Note most systems will allow 127.0.0.1 but some will not .

minerd --url=http://127.0.0.1:36890 --userpass=rpcusername:rpcpassword
minerd --url=http://localhost:36890 --userpass=rpcusername:rpcpassword
minerd --url=http://externalip:36890 --userpass=rpcusername:rpcpassword

# Alex-coin
UBUNTU:
```
git clone 
https://github.com/says112/Alex-coin.git
```
```
cd alexcoin
```
Create an Alex$ coin wallet: 1: Create a wallet using the command:
 ```
./geth --datadir node account new
 ```
2: Install the genesis block:
 ```
./geth init --datadir node genesis.json
 ```
In the node folder, create a pass file and write down the password of the wallet account. Run: 
```
./geth --datadir node --port 30306 --nodiscover --networkid 6699 --unlock <Your wallet> --password node/pass --http --http.addr 127.0.0.1 --authrpc.port 8547 --mine --miner.etherbase <Your wallet> --allow-insecure-unlock --syncmode "full" --snapshot=false --config .config
```
Metamask Wallet:
1 Add Alex$ network to matamask:
Network Name:
 ```
Alex$ network
 ```
New RPC URL:
 ```
https://mainet.alexnetwork.space
 ```
Blockchain ID: 
 ```
6699
 ```
Currency symbol:
 ```
ALEX$
 ```
Initialize the genesis block:
```
./geth init -- genesis.json
```
Launch a wallet:
 ```
./geth --nodiscover --networkid 6699 --mine --miner.etherbase <the address of the metamask> --config .config
 ```


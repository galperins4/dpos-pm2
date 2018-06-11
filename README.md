```sh
sudo apt install npm
sudo npm install pm2@latest -g
git clone https://github.com/galperins4/dpos-pm2
cd ~/dpos-pm2
cp node.json ~/ark-node/node.json (change node directory for matching coin)
cd ~/ark-node/
pm2 start node.json --only ark_mainnet (change selection after only for matching coin)
```

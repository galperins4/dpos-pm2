```sh
sudo apt install npm -y
sudo npm install pm2@latest -g
pm2 install pm2-logrotate
pm2 set pm2-logrotate:max_size 500M (set max log size to 500M)
pm2 set pm2-logrotate:retain 2 (retain 2 copies)
git clone https://github.com/galperins4/dpos-pm2
cd ~/dpos-pm2
cp node.json ~/ark-node/node.json (change node directory for matching coin)
cd ~/ark-node/
pm2 start node.json --only ark_mainnet (change selection after only for matching coin)
```

# Solar Block Producer guide
⚠️Only try to become a Block Producer for Solar if you know how to run a secure and stable server. ⚠️

## Testnet
### Get some Testnet SXP
First try all this on Testnet to know you understand everything and everything is working.
Get some testnet SXP (tSXP) to be able to register a block producer on testnet. [Testnet Telegram Faucet Bot](https://t.me/dSXP_bot)

### Setup 2 nodes
Follow the [official node installation guide](https://docs.solar.org/exchanges/node-installation/requirements/) to setup 2 **testnet** nodes. 
- one will be used for the actual block producing on testnet
  - Instead of the mentioned port 6001, open port 6002 for testnet. On mainnet you do need to open port 6001.
- one will be used to distribute rewards to your voters
  - Don't open any of the mentioned ports 

Check with `pm2 logs` if the block height in the logs is equal to the [height of testnet](https://testnet.solarscan.com/).
When the height is the same, your node is in sync. It will probably at take a few hours before your node is in sync with the network.

### Register your Block Producer
Go into your wallet in the Solar Desktop Wallet and click the three dots -> Registration -> Register Delegate.
And enter the name by which you want your Block Producer to be known.

### Configure your block producer in one of your nodes
⚠️ Don't do this step as long as your node is not in sync.⚠️
Choose one of the servers where you installed the Solar testnet node to configure your 
Type `solar config:forger`. 
Choose BIP39 and enter your passphrase. 
After that type `solar forger:start`. 
Your Testnet Block Producer should now be running.

### Configure cactus-tbw in your other node
⚠️ Don't do this step as long as your node is not in sync.⚠️
Follow the [cactus-tbw installation guide](https://github.com/Cactus-15-49/cactus-tbw) to install cactus-tbw on you other node. Cactus-tbw will be used to give your voters a part of the rewards you receive for producing blocks.

### Ask for a vote
When everything is configured and running correctly. Ask for a vote in the testnet discord channel, so your Block Producer can be voted in the top 53 and become an active Block Producer.

## Mainnet
⚠️⚠️Take your time to monitor if everything is going ok on Testnet before thinking about going to mainnet.
You don't want to make mistakes on mainnet, because if can impact the security and stability of the network.⚠️⚠️
To be continued...

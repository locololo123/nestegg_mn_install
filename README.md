<h1>NestEGG Masternode Setup Guide</h1>
<h2>Prerequisites:</h2>

VPS running Ubuntu 18.04: 1 CPU, 25GB Storage, 1024MB Ram (You can obtain through Vultr if you do not have your own.)
https://www.vultr.com/?ref=8633741

25,000 NestEGG Coins + a few extra for fees

Synced QT Wallet

Running Ubuntu 18.04 use:

git clone https://github.com/locololo123/nestegg_mn_install.git && cd nestegg_mn_install && sudo chmod +x MN_Script.sh && bash MN_Script.sh

<h3>Verify node status</h3>

<p>Wait until your masternode is fully Synced with blockchain. You can check this with the command below:</p>

 nestegg-cli getinfo
<p>When your masternode is fully synced enter the command below to verify your masternode status:</p>

 nestegg-cli getmasternodestatus
 
<h3>QT Wallet commands to start Masternode</h3>

Type the following in the Debug Console (Make sure your Collateral transaction has at least 15 confirmations).

<p> startmasternode alias 0 "masternode alias name"
      example: startmasternode alias 0 mn1</p>

***

<p align="center">
  <img width="760" height="315" src="https://imgur.com/tQQkMPn.png/760/315">
</p>

***

***This guide is for updating existing ZelNodes that were installed using the VPS script and a ZelCash full node on ZelCore.  Use Goose's video guide in conjection to help answer any questions by clicking [here](https://www.youtube.com/watch?v=NNWgBzEl_TI)***

***

***If you require further assistance contact the support team on [Discord](https://discord.gg/szN9yZ) or [Telegram English](http://t.me/zelcash) / [Chinese](http://t.me/zelcashcn) / [Russian](http://t.me/zelcashru)***

***

## SECTION A: UPDATING VPS
***STEP 1***

***Connect to your VPS using Putty or your terminal of choice***

***PLEASE BE SURE YOU ARE LOGGED IN AS YOUR USERNAME (not root) BEFORE RUNNING THIS SCRIPT***

![Example-PuttyLogin](https://imgur.com/gMkd6fs.png)

***

***STEP 2***

***Run update script***

`wget -O zelnodeupdate.sh https://raw.githubusercontent.com/zelcash/ZelNodeUpdate/master/zelnodeupdate.sh && chmod +x zelnodeupdate.sh && bash ./zelnodeupdate.sh`

***HUGE SHOUTOUT TO GOOSE, SKYSLAYER AND DK808 FOR PUTTING TOGETHER THIS INSTALL SCRIPT***

***

***STEP 3***

***Reboot once the script has finished installing by running the following command***

`sudo reboot -n`

***

***STEP 4***

***Log back into your VPS and verify the download is showing 'protocolversion 170010' and 'blocks' matches the current block***

***Run this command to see the info***

`zelcash-cli getinfo`

![Example-OS](https://imgur.com/PLxhNBy.png)

***Check the current block on the explorer by clicking [here](https://explorer.zel.cash/blocks)***

***

## Section B: Updating ZelCore and Starting ZelNode(s)
***STEP 1 (if necessary)***

***Log into ZelCore to auto update to the new bins and reboot to install them***

***

***STEP 2***

***Open your ZelCore wallet and choose 'ZelCash'***

![Example-OS](https://imgur.com/9WrruJR.png)

***

***STEP 3***

***'Full Node'***

![Example-OS](https://imgur.com/CXLLEth.png)

***

***STEP 4***

***'Launch Full Node'***

![Example-OS](https://imgur.com/EvEj6H2.png)

***

***STEP 5***

***'Launch ZelCash' when prompted*** 

![Example-OS](https://imgur.com/PbIIEt9.png)

***

***STEP 6***

***Go into 'Tools' after wallet is 100% synced***

![Example-OS](https://imgur.com/uvqjVZ6.png)

***

***STEP 7***

***'ZelNodes Management'***

![Example-OS](https://imgur.com/J7TqUmN.png)

***

***Step 8***

***'Start ZelNodes'***

***MAKE SURE TO ONLY START ZELNODES THAT HAVE BEEN UPDATED ON THE VPS SIDE***

![Example-OS](https://imgur.com/mejUwOs.png)

***

***STEP 9***

***Go back to your VPS to confirm that your ZelNode is showing 'Status 4' by running the following command (If it does not show successfully started, wait 5 minutes and run the command again. Repeat if necesary)***

`zelcash-cli getzelnodestatus`

![Example-installing](https://imgur.com/nj76J7D.png)

***You can also view your ZelNode on the [block explorer](https://explorer.zel.cash/zelnodes)***

![Example-installing](https://imgur.com/SkGqa6D.png)

***It will show up as 'PRE_ENABLED' prior to 15 confirmations at a minimum, and it could take several hours to show as 'ENABLED'***

***

***CONGRATULATIONS AND THANK YOU FOR BEING A PART OF THE COMMUNITY!!!!!!!!!!!!!***

***






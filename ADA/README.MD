# Cordana


### Wallet Software

There is a wallet called [Yoroi](<https://chrome.google.com/webstore/detail/yoroi/ffnbelfdoeiohenkjibnmadjiehjhajb/related>) that runs as a Chrome App and can be used to offline generate keypairs. 

1. Navigate to <https://chrome-extension-downloader.com/> and enter the URL of Yoroi: `https://chrome.google.com/webstore/detail/yoroi/ffnbelfdoeiohenkjibnmadjiehjhajb/related`
2. Click *Download extension*
3. Ignore the warning and save the file (Yoroi_v1.0.2.crx)
4. Get the source code by dropping the .crx file on <http://crxextractor.com/>
5. Extract the downloaded Zip (take it to your Airgapped PC)
6. Rename the extracted directory to `Yoroi_v1.0.2`
7. Inside this directory, rename the `_metadata` directory to `metadata`
8. Open Chrome and navigate to <chrome://extensions/>
8. Select 'Developer mode' and Click *Load extracted extension* and point to the directory. This should install the app.
9. Navigate to <chrome://apps> and start the ICONEX chrome app.

### Offline Address Generation

1. Start Chrome and the Yoroi extension.
2. Click *Create Wallet*
4. Think of a Wallet Name and a password, confirm it, click *Create personal wallet*.
5. Check the checkbox and click *Continue*.
6. Register the mnemonic (use rightclick inspect to copy it)
6. Click *Yes I have written it down*
7. Re-enter the mnemonic, and check the boxes
8. Click *Confirm*
9. Click on *Receive*
10. Register the Address

### Using the Address Online

1. Start Chrome and the Yoroi extension.
2. Click *Load Wallet*
3. Select *Enter the mnemonic* and think of a password
4. Click *Send*
5. Enter address, amount and password, click *Send*
6. Wait for it to be confirmed




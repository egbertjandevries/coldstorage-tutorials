# Tezos
---
### Wallet Software

There is a wallet [TezBox](<https://chrome.google.com/webstore/detail/tezbox-tezos-wallet/mnfifefkajgofkcjkemidiaecocnkjeh>) that runs as a Chrome App and can be used to offline generate keypairs. 

#### Installing TezBox on an airgapped PC with Chrome 

1. Navigate to <https://chrome-extension-downloader.com/> and enter the URL of TezBox: `https://chrome.google.com/webstore/detail/tezbox-tezos-wallet/mnfifefkajgofkcjkemidiaecocnkjeh`
2. Click *Download extension*
3. Ignore the warning and save the file (TezBox-Tezos-Wallet_v9.0.0.crx)
4. Get the source code by dropping the .crx file on <http://crxextractor.com/>. 
5. Move the ZIP file to the airgapped PC.
5. Extract the downloaded `ZipTezBox-Tezos-Wallet_v9.0.0`
7. Inside this directory, rename the `_metadata` directory to `metadata`
8. Open Chrome and navigate to <chrome://extensions/>
8. Select 'Developer mode' and Click *Load extracted extension* and point to the directory. This should install the app.
9. Navigate to <chrome://apps> and start the ICONEX chrome app.

### Offline Address Generation using TezBox

1. Start Chrome and the TezBox extension.
2. Click *CREATE TEZBOX*
3. Register the words (mnemonic) that make up the seed phrase and an register them.
4. Click *CREATE*
5. Re-enter the words and think of a (dummy) password
6. Click *ENCRYPT*
7. Register the address that is found under MAIN, starting with `tz...`
8. You might want to register the bare private key as well, to have a second Restore option. Go to Settings and Enter the password you used earlier.
9. Register the private key.

### Using the Address Online
1. Start Chrome and the TexBox extension
2. If you have used it before click *Clear TezBox* first
3. Click *Restore TezBox*
4. Enter the mnemonic and click *RESTORE TEXBOX*. Alternatively you could restore by *PRIVATE KEY*, and click *RESTORE TEZBOX*.
5. Think of a (dummy) password and enter it twice, click on *DECRYPT*.
6. Now you are in the wallet. Click on Send to transfer.

### Offline Transaction Signing
Read [here](https://medium.com/@KukaiWallet/setting-up-an-offline-wallet-with-kukai-6a6ca5cd6a36) how to do it.

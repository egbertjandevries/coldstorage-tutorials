There are two ways to safely handle Tezos funds. Using offline transaction signing (preferred), or using throw away addresses. Both are described here.

# Offline Transaction Signing using Kukai
Read [here](https://medium.com/@KukaiWallet/setting-up-an-offline-wallet-with-kukai-6a6ca5cd6a36) how to do it.

### 0. Create wallet:

#### ONLINE SYSTEM:
1. download Kukai
1. Apply checksum
1. Copy to offline system

#### OFFLINE SYSTEM:
1. Install Kukai and start app
1. Create new wallet
1. Create entropy
1. Administer seed
1. Administer public key
1. download encrypted keystone file (you can cancel this, file isn't needed)
1. Go to 'backup' section
1. Export View-only wallet to file using the password
1. scan the contents of the file with the scanner to the online PC

### 1. Create unsigned operation:
#### ONLINE SYSTEM:
1. Put the scanned content in a *.tez wallet file
1. Load the wallet file in Kukai
1. In Overview section of Kukai wallet, create a transaction (send)
1. Select the From Address
1. Insert the To Address
1. Insert the Amount to Send and the Fee
1. Click on preview
1. Insert the password and click on confirm
1. a file with the extention .tzop is created
1. Open the .tzop file and copy the unsigned operation to the QR software
1. Scan the QR code to the offline PC

### 2. Sign operation offline:
#### OFFLINE SYSTEM:
1. In Kukai app, go to the Offline signing section
1. In Sign operation (offline), insert the unsigned operation
1. Insert the password and click on sign
1. Download the signed.tzop file and open it
1. Put the hex in the QR app and scan it to the online PC

### 3. Broadcast the transaction:
#### ONLINE SYSTEM:
1. In Kukai app, go to the Offline signing section
1. In Broadcast (online), insert the hex and click on broadcast
1. You get a message: "do you want to decode", ignore this (otherwise, it will not work)
2. Register the transaction id for checking it on [tzscan.io](<http://www.tzscan.io>)

----------------------

# Using Tezbox and throw-away addresses
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


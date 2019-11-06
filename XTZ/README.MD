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

# Using Tezbox with ledger support

### Wallet Software

There is a wallet [TezBox](<https://github.com/tezbox/desktop-wallet/releases>) that runs as a standalone app on Windows or MacOS. 

#### Using TezBox app with ledger

1. Navigate to <https://support.ledger.com/hc/en-us/articles/360016057774-Tezos-XTZ-> and follow the instructions to install the app
2. Navigate to <https://medium.com/@obsidian.systems/getting-started-with-tezos-on-the-ledger-nano-s-c011517b0f3c> and scroll down to the instructions for TezBox to connect the ledger
3. Delegation cabn be done through the 'delegate' tab in the TezBox app. Explanation on how to delegate safely can be found here: <https://medium.com/cryptium/how-to-store-your-tezos-xtz-in-your-ledger-nano-s-and-delegate-with-tezbox-wallet-8fb4ac2d3355>


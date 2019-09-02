# RVN

### Wallet Software

For offline address generation and offline transaction signing we use the [PocketRaven Webwallet](https://pocketraven.com/#home) and the offline version.

To download an offline version, navigate to [https://github.com/traysi/pocketraven](https://github.com/traysi/pocketraven) and save the project as a ZIP. 

To run it offline, unzip it on a offline PC and load the index.html.

### Offline Address generation

1. Load the `../pocketraven-master/index.html` file in a browser on an offline PC.
2. Click on *New*
3. Click on *Generate*. Keep *Compress* checked
4. Register the
2. Generate enough entropy by moving the mouse or enter the keys
3. Click on *Print Front*
4. Register the Public Key and the Private Key and the Address(the upside down one)

### Offline Transaction Signing

1. Start the [Online Wallet](https://pocketraven.com/#newTransaction)
2. Enter the Public Address from which you want to transfer and click *Load*.
3. Enter the Address and Amount for the transaction.
4. Click *Submit*
5. Transfer the unsigned transaction to the offline PC
6. Load the offline wallet `../pocketraven-master/index.html` and go to *Sign*
7. Paste the Primary Key together with the unsigned transaction and click *Sign*
8. Transfer the signed transaction back to the online PC and paste it into *Broadcast*


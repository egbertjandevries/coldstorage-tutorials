## EOS

### Wallet Software

There is a wallet for offline address generation. 

There is a an adress generator here: <https://nadejde.github.io/eos-token-sale/#>.
Follow there steps to run it offline:

1. Navigate to <https://nadejde.github.io/eos-token-sale/#>
2. Save the site using Save as HTML to your local filesystem
3. Open de file `EOS Key Generation.html` using Firefox, or boot Chrome without cross-browser security:
	*  on OSX: `open -a Google\ Chrome --args --disable-web-security --user-data-dir` 
	*  on Windows: `chrome.exe" --disable-web-security --user-data-dir="C:/gebruikers/gebruiker`
4.  Open the file `EOS Key Generation.html` from the filesystem, using Chrome

A different option

4. Fire up a webserver, e.g: `python -m SimpleHTTPServer 8000`
5. In offline mode, run the generator locally on OSX: <http://localhost:8000/EOS%20Key%20Generation.html>


#### Online Wallet
As online wallet we can use the Scatter plugin for Firefox or Chrome. Get it [here](https://get-scatter.com/), which we can use in combination with the EOS toolkit - <https://eostoolkit.io/account/permissions>.

### Offline Address generation

1. Having loaded the `EOS Key Generation.html` in your browser (Firefox or Chrome with disabled security), click on *Generate EOS Key*
2. Register the Private and Public Key.

### Sending funds using Scatter and EOS Toolkit
EOS works with accounts as a primary actor. The EOS blockchain registers two Public Keys with every account, `owner` and `active`.
First we need to make sure to have a different @owner and @active address.

The idea is to never change the `@owner` Public Key and never expose the corresponding Private Key and use the `@active` Public Key to transfer funds and replace it everytime it's Private Key has been exposed.

#### Check Active and Owner Public Keys

1. Start [EOS Toolkit](<https://eostoolkit.io/account/permissions>),
2. Go to *Find Account* and supply the account name `gi4tambtg4ge` *Search Account* and click *Search*.
3. Once found, click on `Show Json` and check the keys with `active` and `owner`. 

#### Transfer Funds
1. In Scatter, register the active `@active` Public Key  under Key Pairs. 
2. Click *New*, name it `Active Key` and enter the corresponding Private Key. Click *Save*.
3. Still in Scatter, navigate to Identities and click *Create Identity*.
4. With Account, select `EOS Mainnet` and below, select `Active Key`. Click *Import*. 
5. On Select Account, select the `gi4tambtg4ge@active` and click *Use Selected Account* and click *Save*.
6. Navigate to <https://eostoolkit.io> and click on *Connect Account*. 
7. Scatter pops up. Select the EOS account `gi4tambtg4ge@active` and click `select identity` and click *Accept*. The account name appears in the left upper corner of EOS Toolkit.
8. Select *Transfer EOS*.
9. Supply Quantity, Recipient and the Memo and click *Send*.
10. *Accept* in Scatter.

#### Replace Public Key
Be sure the connect the account using steps 1-7 above.

1. In EOS Toolkit, navigate to *Manage Account*, *Manage Permissions*.
2. Enter the Public Key that comes with the next active address and supply it in the *Active Permission* field. Leave the other field empty.
3. Click *Update*.
4. Scatter comes up. Click *Accept*.
5. Check if the new active Public Key has become the active one using the procedure described above.


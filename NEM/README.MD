# NEM

### Wallet Software

For NEM we use the [NanoWallet](https://github.com/NemProject/NanoWallet/releases)

For Linux
1. Download it
2. After downloading, check the checksum with `openssl sha -sha256 NanoWallet-1.4.13-osx64.zip`
3. Expand the ZIP

For Windows:
1. Download the Checksum program at: http://www.microsoft.com/en-us/download/details.aspx?id=11533
2. After downloading the checksum program, install it in C:\Windows\System32\
3. Download the NEM wallet
4. CMD as admin= `C:\Windows\System32\CertUtil -hashfile ...\NanoWallet-1.4.13-win64.zip SHA256`
5. Expand the ZIP



### Offline Address Generation

We don't use the BIP32 feature but create the addresses with a separate private key each.

Following steps:

1. Start the wallet by loading the `start.html` from the wallet distro in a browser.
2. Choose *Signup* and click *Simple Wallet*.
3. Enter a unique wallet name, select *Mainnet*, and choose a password (can be 'dummy')
4. Save the dummy wallet file.
5. Click on *Show private key* in the next dialog and register the key in the NEM address list.
6. Refresh the page.
7. Click on *Private key wallet* and enter the private key.
8. The public address shows up, register it.



### Using the Address online

1. Start the wallet by loading *start.html* from the NanoWallet distro
2. Select *Signup* and click *Private Key Wallet*
3. Enter a wallet name and a password, memorize it.



### Cold Transaction Signing

There is possibility using [this project](https://github.com/rb2nem/nem-offline-signer). It works with Groovy.








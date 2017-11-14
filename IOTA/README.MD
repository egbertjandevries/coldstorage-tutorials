# IOTA

### Wallet Software

IOTA Wallets can be downloaded [here](https://github.com/iotaledger/wallet/releases). 

For paper wallet generation [this tool](https://arancauchi.github.io/IOTA-Paper-Wallet/ ) is available. Click on *Download an offline version of this site*.

For Windows:
1. Download the Checksum program at: http://www.microsoft.com/en-us/download/details.aspx?id=11533
2. After downloading the checksum program, install it (right click: run as administrator) in C:\Windows\System32\
3. Download the IOTA wallet
4. After downloading, check the checksum with: CMD as admin= `C:\Windows\System32\CertUtil -hashfile ...\IOTA.Wallet.Setup.2.5.4.exe SHA256`
5. Download the PWGen password generator at: http://pwgen-win.sourceforge.net/
6. Copy the offline wallet software and the PWGen tool to the airgapped PC and Install both



### Offline Address generation

1. Start the PWGen tool and generate a seed of lenght 81 using Character set: <AZ>9
2. Start the address generator by loading the *index.html* in a browser.
3. Enter and Register the SEED.
4. Register the address together with the SEED.

   ​

### Using the Address online

1. Start the IOTA wallet
2. Enter the SEED
3. Check the corresponding address
4. Mark the SEED as used.



### Cold Transaction Signing

As yet, not available for IOTA


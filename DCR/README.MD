# Decred
-

### Wallet Software

There is an offline paper wallet `dcraddreg.exe` that has to be build from this [repo](https://github.com/decred/dcraddrgen) using the Go language.

As online wallet, use the Decredition wallet, download it here <https://www.decred.org/downloads/>.

### Offline Address Generation

1. In a commandline, run the `dcraddrgen.exe`.
2. Register the `seed` and the `Hex version` of the seed. 
3. Save the text file.
4. Open it and register the `first address` and the `extended public key`

### Using the address online

1.  Open the Decredition wallet and choose *New Wallet*.
2. Think of a username.
3. Choose *Restore*
4. Enter the `seed` or the `Hex version` and think of a private passphrase.
5. Click on *Create Wallet*
5. Wait for the wallet to sync.
6. Use the passphrase and click *Scan* to scan the blockchain 
6. When finished, click on *Transactions*
7. Use *Send*

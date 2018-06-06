# XMR

### Wallet Software

There is an online Monero wallet available at <https://mymonero.com/#/>. You can log in there using a mnemonic or a combination of a public key, view key and spend key.

An online Desktop Wallet can be found here <https://getmonero.org/downloads/#windows>

For offline address generation we use this HTML file: <https://github.com/moneromooo-monero/monero-wallet-generator/>

### Offline Address generation

1. Start the offline wallet generator
2. Click *Generate Wallet*.
3. Register the Public Address, the mnemonic, the spend key and view key.

### Using the Address online

1. Start the Online Wallet, Monero Wallet GUI, choose English
2. Choose *Restore wallet from keys*
3. Enter the keys and a suitable block height as close as possible to the date that the old address started to be used. Check [here](<https://moneroblocks.info/search/1572000>).
4. Deamon needs to synchronize first…. can take some time. Choose External Node from `https://moneroworld.com/` e.g. `ushouldrunyourownnode.moneroworld.com` at port `18089`.
5. Send can only be done on synchronized Monero chain

### Cold Transaction Signing

Possible as described in this post <https://monero.stackexchange.com/questions/2160/how-do-i-use-cold-transaction-signing>
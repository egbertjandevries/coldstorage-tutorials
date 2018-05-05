## EOS

### Wallet Software

EOS has not mainnet yet, and no official Wallet software. 
But there is a wallet for offline address generation. EOS mainnet addressen need to be generated and mapped to the EOS ERC-20 tokens to the mainnet addresses, before the 3rd of July 2018. 
Read [here](<https://steemit.com/eos/@sandwich/contributing-to-eos-token-sale-with-myetherwallet-and-contract-inner-workings>) how to do it.

There is a an adress generator here: <https://nadejde.github.io/eos-token-sale/#>.
Follow there steps to run it offline:

1. Navigate to <https://nadejde.github.io/eos-token-sale/#>
2. Save the site using Save as HTML to your local filesystem
3. Open de file `EOS Key Generation.html` using Firefox, or boot Chrome without cross-browser security:
	*  on OSX: `open -a Google\ Chrome --args --disable-web-security --user-data-dir` 
	*  on Windows: `chrome.exe" --disable-web-security`
4.  Open the file `EOS Key Generation.html` from the filesystem, using Chrome

A different option

4. Fire up a webserver, e.g: `python -m SimpleHTTPServer 8000`
5. In offline mode, run the generator locally on OSX: <http://localhost:8000/EOS%20Key%20Generation.html>


### Online Wallet
[not available yet]

### Offline Address generation

1. Having loaded the `EOS Key Generation.html` in your browser (Firefox or Chrome with disabled security), click on *Generate EOS Key*
2. Register the Private and Public Key.

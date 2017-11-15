# WAVES

### Wallet Software

The light client [WavesLiteApp](https://chrome.google.com/webstore/detail/wavesliteapp/kfmcaklajknfekomaflnhkjjkcjabogm) that runs as a Chrome App is the best option, it can be used to generate paper wallets, though it can't be used for cold transaction signing, afaik.

To install the the WavesLiteApp on an offline PC we first need to load the App as a CRX file. 

1. Navigate to <https://chrome-extension-downloader.com/> and enter the URL of the WavesLiteApp: https://chrome.google.com/webstore/detail/wavesliteapp/kfmcaklajknfekomaflnhkjjkcjabogm
2. Click *Download extension*
3. Ignore the warning and save the file (WavesLiteApp_v0.5.7.crx)
4. Get the source code by dropping the .crx file on <http://crxextractor.com/>
5. Extract the downloaded Zip
6. Rename the extracted directory to `WavesLiteAppv0.5.7`
7. Inside this directory, rename the `_metadata` directory to `metadata`
8. Open Chrome and navigate to <chrome://extensions/>
9. Select 'Developer mode' and Click *Load extracted extension* and point to the directory.
10. Navigate to <chrome://apps> and start the WavesLite client



### Offline Address Generation

1. Start the WavesLite client from <chrome://apps> 
2. Click *NEW ACCOUNT*
3. Think of a Name and a Password
4. In the Wallet Screen, click on the Backup Icon in the right upper screen.
5. Now, register the Seed, the Encoded Seed, the Private Key, the Public Key, Address



### Using the Address online

1. Start the WavesLite client from <chrome://apps>
2. Click import account
3. Paste in the Seed.
4. Think of a Name and a Password
5. Click *Register*
6. Click on *Send* under Waves



### Cold Transaction Signing

Not supported




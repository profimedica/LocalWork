This doc contain one-time settings

Sign Application and extract key for google and facebook
Extract openssl from 

"C:\Program Files\Java\jdk1.7.0_79\bin\keytool" -list -v -keystore "D:\AndroidStudioProjects\LocalWork3\LocalWork.jks"
This refult is for Google Play Services:

7A B7 BE 10 EE 15 51 3F 0A 4A E4 1B A6 99 E4 CF AA AA 2F 37

"C:\Program Files\Java\jdk1.7.0_79\bin\keytool" -exportcert -alias LocalWork -keystore "D:\AndroidStudioProjects\LocalWork3\LocalWork.jks" | "D:\AndroidStudioProjects\LocalWork3\EraseThisLater\bin\openssl" sha1 -binary | "D:\AndroidStudioProjects\LocalWork3\EraseThisLater\bin\openssl" base64
Result for https://developers.facebook.com/apps will also be contained in the login error message on your android phone
GnQBnVRRq8FJsVAIgdkc9K+fk/8=
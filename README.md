Useful Commands:
keytool -genkeypair -keyalg "RSA" -keysize 2048 -alias baeldungspringsaml -storepass baeldungsamlokta -keystore keystore.jks

keytool -v -export -file mytrustCA.cer -keystore keystore.jks -alias baeldungspringsaml -storepass baeldungsamlokta

keytool -importcert -alias baeldungspringsaml_azure -storepass baeldungsamlokta -keystore keystore.jks -file azure_ad.cer

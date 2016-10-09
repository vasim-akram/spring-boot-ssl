# spring-boot-ssl
This app configure with ssl/tls configuration.

# Enable HTTPS in spring boot app
     keytool -genkey -alias tomcat (this command available in already java installed systm)
     -storetype PKCS12 -keyalg RSA -keysize 2048
     -keystore keystore.p12 -validity 3650

    Enter keystore password:
     Re-enter new password:
     What is your first and last name?
     [Unknown]:
     What is the name of your organizational unit?
     [Unknown]:
     What is the name of your organization?
     [Unknown]:
     What is the name of your City or Locality?
     [Unknown]:
     What is the name of your State or Province?
     [Unknown]:
     What is the two-letter country code for this unit?
     [Unknown]:
     Is CN=Unknown, OU=Unknown, O=Unknown, L=Unknown, ST=Unknown, C=Unknown correct?
     [no]: yes
# Update application.properties file
    server.port: 8443
    server.ssl.key-store: keystore.p12
    server.ssl.key-store-password: mypassword
    server.ssl.keyStoreType: PKCS12
    server.ssl.keyAlias: tomcat
# For enable HTTPS in spring boot 
   * [https://www.drissamri.be/blog/java/enable-https-in-spring-boot/]

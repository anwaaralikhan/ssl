
> keytool is a key and certificate management utility that we will use to create our private keys and certificates. Keytool comes with the standard JDK Distribution. The following example of JConsole SSL connection uses the keyool library from JDK 8.

### Step 1: Generate key pair on Server or the Host machine (JMX Agent – Server).
Current Directory (Server): B:\JMX\Security

```
B:\JMX\Security>keytool -genkeypair -keystore serverkeystore -alias serverkey -validity 180 -storepass serverpass -keypass serverpass
What is your first and last name?
  [Unknown]:  JMX Agent
What is the name of your organizational unit?
  [Unknown]:  DevOps
What is the name of your organization?
  [Unknown]:  CleanTutorials
What is the name of your City or Locality?
  [Unknown]:  Delhi
What is the name of your State or Province?
  [Unknown]:  Delhi
What is the two-letter country code for this unit?
  [Unknown]:  IN
Is CN=JMX Agent, OU=DevOps, O=CleanTutorials, L=Delhi, ST=Delhi, C=IN correct?
  [no]:  yes
```

```
B:\JMX\Security>keytool -genkeypair -keystore serverkeystore -alias serverkey -validity 180 -storepass serverpass -keypass serverpass
What is your first and last name?
  [Unknown]:  JMX Agent
What is the name of your organizational unit?
  [Unknown]:  DevOps
What is the name of your organization?
  [Unknown]:  CleanTutorials
What is the name of your City or Locality?
  [Unknown]:  Delhi
What is the name of your State or Province?
  [Unknown]:  Delhi
What is the two-letter country code for this unit?
  [Unknown]:  IN
Is CN=JMX Agent, OU=DevOps, O=CleanTutorials, L=Delhi, ST=Delhi, C=IN correct?
  [no]:  yes
 ```
Since we are creating a self-signed certificate,  after entering the command the tool will ask us about the details of the certificate such as the first and last name. You can fill out random information for development purpose. After filling the information, it will create a “serverkeystore” file in the current directory

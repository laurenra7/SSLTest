# SSLTest
Test servers for SSL/TLS protocol and cipher support. The code is written by Christopher Schultz. See original code at:

[SSLTest.java](https://wiki.apache.org/tomcat/tools/SSLTest.java)
[SSLUtils.java](https://wiki.apache.org/tomcat/tools/SSLUtils.java)

### Build

Build with [Maven](https://maven.apache.org/).

```
mvn clean install
```

Produces an executable .jar file

```
/target/SSLTest.jar
```


### Run

```
java -jar SSLTest.jar
```


### Options

```
Usage: java class org.la.util.SSLTest [opts] host[:port]

-sslprotocol                 Sets the SSL/TLS protocol to be used (e.g. SSL, TLS, SSLv3, TLSv1.2, etc.)
-enabledprotocols protocols  Sets individual SSL/TLS ptotocols that should be enabled
-ciphers cipherspec          A comma-separated list of SSL/TLS ciphers
-truststore                  Sets the trust store for connections
-truststoretype type         Sets the type for the trust store
-truststorepassword pass     Sets the password for the trust store
-truststorealgorithm alg     Sets the algorithm for the trust store
-truststoreprovider provider Sets the crypto provider for the trust store
-no-check-certificate        Ignores certificate errors
-no-verify-hostname          Ignores hostname mismatches
-h -help --help     Shows this help message
```

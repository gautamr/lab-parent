Parent POM file for all lab maven projects/artifacts.

Please note that for deployment of aritfact we are using [Apache Maven GPG Plugin](http://maven.apache.org/plugins/maven-gpg-plugin/)
This is true for this parent POM.

So to install this file in local Maven repo do the following:

### 1 Install
    [GPG for Windows] (https://www.gpg4win.org/download.html) if you are using windows.
### 2 Verify the installation by
    gpg --version
### 3 Generate a Key Pair
    gpg --gen-key
Provide passphrase when promoted
### 4 Install using maven
    mvn clean install -Dgpg.passphrase=<yourpassphrase> -Dgpg.keyname=<keyname>


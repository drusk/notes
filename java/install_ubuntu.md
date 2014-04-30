Install Oracle Java 7
---------------------
```
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java7-installer
```

Install Oracle Java 8
---------------------
```
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update
sudo apt-get install oracle-java8-installer
```

Switching Between Versions
--------------------------
Switch to Java 7:
```
sudo update-java-alternatives -s java-7-oracle
```

Switch to Java 8:
```
sudo update-java-alternatives -s java-8-oracle
```

Check Java Version
------------------
```
java -version
```

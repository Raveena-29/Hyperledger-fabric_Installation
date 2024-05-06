# Hyperledger Fabric Tnstallation

# Prerequisites

1. cURL — latest version
 
2. Docker — version 17.06.2-ce or greater

3. Docker Compose — version 1.14.0 or greater

4. Golang — version 1.11.x

5. Nodejs — version 8.x (other versions are not in support yet)

6. NPM — version 5.x

7. Python 2.7

 * A) Add the new user “fabric”
   
```
sudo adduser fabric
```

* B) Add the user “fabric” to the Sudo groups

```
sudo usermod -aG sudo fabric
```

* C) Login to “fabric” user

```
su fabric
```

* D) Test the sudo access

```
sudo ls
```

* E) check your curl , docker, docker-compose , go , python , npm , nodejs version
  

# Install Samples, Binaries and Docker Images

* A) Make the directory where you want to install the fabric-samples

```
mkdir file(in my case)
cd file
```

* B) Determine the directory where you want to download the fabric samples. Open the directory in terminal and run the below command.

```
curl -sSL http://bit.ly/2ysbOFE | bash -s
```


* C) Open the fabric-samples and go to the first-network.

```
cd fabric-samples/first-network
```


* D) To test it, run the `network.sh` . It is a test script, it first set up the network with 2 organizations org1 and org2 with 2 peers each and an orderer .


```
sudo ./network.sh up
```




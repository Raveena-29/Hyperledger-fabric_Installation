# Hyperledger Fabric Installation

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
![blockchain5](https://github.com/Raveena-29/Hyperledger-fabric_Installation/assets/148243757/0409e782-09d4-44de-908d-301e12ee0fbf)

* B) Determine the directory where you want to download the fabric samples. Open the directory in terminal and run the below command.

```
curl -sSL http://bit.ly/2ysbOFE | bash -s
```
![blockchain2](https://github.com/Raveena-29/Hyperledger-fabric_Installation/assets/148243757/4d93210d-8b8d-477d-8a36-ff2b439e6006)
![blockchain3](https://github.com/Raveena-29/Hyperledger-fabric_Installation/assets/148243757/87d9a4df-0ba2-4fc2-bafa-72b4ae7b89d9)

* C) Open the fabric-samples and go to the test-network.

```
cd fabric-samples/test-network
```


* D) To test it, run the `network.sh` . It is a test script, it first set up the network with 2 organizations org1 and org2 with 2 peers each and an orderer .


```
sudo ./network.sh up
```

![Capture](https://github.com/Raveena-29/Hyperledger-fabric_Installation/assets/148243757/70fecd22-ff21-4dee-91d7-68a680858342)


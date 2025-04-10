# Hyperledger Fabric Test Network Setup

This project explains how to set up and run a basic Hyperledger Fabric test network using its official sample repository. It includes installing the required tools, downloading the Fabric samples, and using the `network.sh` script.

---

## Prerequisites Installation

### 1. Install Go (Golang)
Go is needed to build Fabric binaries.

```bash
sudo apt install golang-go
```

**Screenshot:**

![Go Version](images/step1_go_version.png)

---

### 2. Check Docker Installation

```bash
docker --version
```

**Screenshot:**

![Docker Version](images/step2_docker_version.png)

---

### 3. Check Docker Compose Installation

```bash
docker-compose --version
```

**Screenshot:**

![Docker Compose Version](images/step3_docker_compose_version.png)

---

### 4. Verify Directory Structure

Check the current directory structure:

```bash
ls
```

**Screenshot:**

![LS Output](images/step4_ls_output.png)

---

## Cloning Fabric Samples

### 5. Clone the Fabric Samples Repository

```bash
git clone -b main https://github.com/hyperledger/fabric-samples.git
```

**Screenshot:**

![Git Clone](images/step5_git_clone.png)

---

### 6. Go to the Fabric Samples Directory

```bash
cd fabric-samples
```

**Screenshot:**

![CD fabric-samples](images/step6_cd_fabric_samples.png)

---

### 7. Download Binaries and Docker Images

```bash
curl -sSL https://bit.ly/2ysbOFE | bash -s
```

**Screenshot:**

![Download Docker Images and Binaries](images/step7_download_docker_imgaes_binaries.png)

---

## Running the Test Network

### 8. Navigate to the Test Network Folder

```bash
cd test-network
```

---

### 9. Start the Network

```bash
./network.sh up
```

**Screenshot:**

![Network Up](images/step9_network_up.png)

---

### 10. Create a Channel

```bash
./network.sh createChannel
```

**Screenshot:**

![Create Channel](images/step8_createChannel.png)

---

### 11. Shut Down the Network

```bash
./network.sh down
```

**Screenshot:**

![Network Down](images/step10_network_down.png)

---

## Conclusion

This setup shows how to install tools and run a basic Hyperledger Fabric test network. It includes starting the network, creating a channel, and stopping everything afterward.

---


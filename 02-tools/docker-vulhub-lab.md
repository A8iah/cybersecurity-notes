 **This command updates the packages in Kali so that we can ensure we install the best updated system, whether it's Docker or any other program, to avoid conflicts with old libraries.**
```bash
 sudo apt update && sudo apt upgrade -y
```
**This is enough; we just need to update the packages in Kali, but not all the packages are the same as the ones above.**
```bash
 sudo apt update
```
**In this matter, we install the Docker in Kali.**
```bash
sudo apt install -y docker.io docker-compose
```
**If we finish and give him a no, there are three commands to check if the program is running or not.**
```bash
1-sudo systemctl start docker
```
```bash
2-sudo systemctl enable docker
```
```bash
3-sudo systemctl status docker
```
**We confirm that this matter is working and what its version is.**
```bash
docker --version
```
**With this matter, we confirm whether it is working or not.**
```bash
docker run hello-world
```
**After that, we will download all the vulnerabilities from this link.**
```bash
git clone --depth 1 https://github.com/vulhub/vulhub.git
```
**After we download the file, we open it this way.**
```bash
cd vulhub && ls
```
**After we downloaded the vulnerabilities file, we run any vulnerability in it this way.**
```bash
cd  We write it here. && ls
```

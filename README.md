### Step 1: Make sure Enable Virtualzation in PC if not enable in BIOS


### Step 2: Install WSL on Windows


1. Opening Windows Powershell Terminal
![Screenshot_357](https://github.com/user-attachments/assets/42e29c7f-9021-433c-87c4-2f76189b1322)

2. Run the WSL Installation Command:
```
wsl --install
```

3. Restart Your Computer:
  
After the installation completes, you may need to restart your computer

### Step 3: Install Ubuntu on Microsoft Store 


### Step 4: Open Ubuntu & Run the script
```
sudo apt update && sudo apt upgrade
```
```
sudo apt install curl
```
```
sudo apt install build-essential
```

### Step 5: Set up the Docker

```
sudo apt-get update
sudo apt-get install ca-certificates curl gnupg
sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg
```

```
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update
```
 Install Docker dependencies
```
sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```
Run hello-world to verify installation

```
sudo docker run hello-world

```

### Step 6: Set up the Ceremony

a - In Browser Signin with GIthub - https://ceremony.union.build/#

b - Choose "Linux" and proceed with required details

c - Copy command in site and paste in to ubuntu panel 

d - Need an Address in the next tab

e - Add UNION TESTNET --- https://chains.keplr.app

f - Connect Keplr Wallet

g - Add Union Network and copy Union address

h - Paste in ceremony tab

### Now your setup complete, Now do not close the browser tab & ceremony tab until your queue completed...

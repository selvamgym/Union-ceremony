## Step 1 Make sure Enable Virtualzation in PC if not enable in BIOS


## Step 2: Install WSL on Windows


1. Opening Windows Powershell Terminal
![Screenshot_357](https://github.com/user-attachments/assets/42e29c7f-9021-433c-87c4-2f76189b1322)

2. Run the WSL Installation Command:
```
wsl --install
```

3. Restart Your Computer:
  
After the installation completes, you may need to restart your computer

## Step 3: Install Ubuntu on Microsoft Store 


## Step 4: Open Ubuntu & Run the script
```
sudo apt update && sudo apt upgrade
```
```
sudo apt install curl
```
```
sudo apt install build-essential
```

### Step 4: Set up the Docker

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
***Optional: To install more packages you can check my recent [Linux guide](https://github.com/0xmoei/Linux_Node_Guide/blob/main/linux-config.md)***

#

## Optional: Change user
There are 2 ways to login to ubuntu: 1. You are `root` (administrator with full permissions), or 2. you are an specific `user` with specific permissions

You see by entering `whoami`, I am logged in as user:mirana

![image](https://github.com/user-attachments/assets/f91fd950-9752-430e-90e1-a7759121d928)


If you want to login with root (full permissions):
```
sudo su
```
![image](https://github.com/user-attachments/assets/2fc310f7-c507-41ac-b116-69ca7d3aa677)


* Now you see I am as `root` user, but in `mirana` user **main** directory
* I need to type `cd` to move to the **main** directory of `root`

***To login to a specific user again, Enter this command:*** `su - username`

#

## Access Ubuntu directories in Windows explorer
To go to your Ubuntu directory using Windows explorer, Enter this in Windows Explorer Addressbar
```
\\wsl$
```

* `home`: main directory of your specific user
* `root`: main directory of your `root` user
![image](https://github.com/user-attachments/assets/87f1fef0-ec1d-4de5-a40e-89a990600c4e)


***If you don't have access to root directory,  Enter this command in terminal*** `sudo chmod 755 /root`







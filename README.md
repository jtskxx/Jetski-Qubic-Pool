# 🌊JETSKI QUBIC POOL🌊

<div align="center">
<h3> <picture> <img src = "https://discords.com/_next/image?url=https%3A%2F%2Fcdn.discordapp.com%2Femojis%2F983705077590130719.gif%3Fv%3D1&w=64&q=75" width = 25px>  </picture> Join us to achieve true AI power powered by useful miners! <img src = "https://discords.com/_next/image?url=https%3A%2F%2Fcdn.discordapp.com%2Femojis%2F983705077590130719.gif%3Fv%3D1&w=64&q=75" width = 25px
	<!--horizontal divider(gradiant)-->
	
<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif">
	<img align="right" width=200px height=200px alt="side_sticker" src="https://media.giphy.com/media/TEnXkcsHrP4YedChhA/giphy.gif" />
</div>

### <a target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/discord.svg" height="30" width="40" /></a> Discord Server: https://discord.jetskipool.ai/


### <picture> <img src = "https://github.com/7oSkaaa/7oSkaaa/blob/main/Images/Statistics.gif?raw=true" width = 30px>  </picture> SOLO Dashboard: https://qubic.jetskipool.ai/
### <picture> <img src = "https://github.com/7oSkaaa/7oSkaaa/blob/main/Images/Statistics.gif?raw=true" width = 30px>  </picture> PPLNS Dashboard: https://pplns.jetskipool.ai/



<br/>



### **⚙️ NVIDIA GPU Requirements:**
> [!NOTE]
> To update your NVIDIA GPU driver on HiveOS, please run the following command:
```sh
nvidia-driver-update
```
- **NVIDIA 3000 Series:** Driver version **535+** or newer.
- **NVIDIA 4000 Series:** Driver version **550+**.


> [!IMPORTANT]
> Ensure each of your workers has a **unique worker name**; duplicating worker names is not permitted.


## ✈️ Flight Sheet Configuration

### Solo Mining➡️ https://github.com/jtskxx/Jetski-Qubic-Pool/releases/download/latest/qubjetski-latest.tar.gz
### PPLNS Mining➡️ https://github.com/jtskxx/Jetski-Qubic-Pool/releases/download/latest/qubjetski.PPLNS-latest.tar.gz
![image](https://github.com/user-attachments/assets/ca0c3dfa-57d1-4df0-b38f-3f1ecbb0a454)


> [!IMPORTANT]
> **For instance: "%WAL%-%WORKER_NAME%"**
>
> **%WAL%-** will use the Qubic wallet address that you configured in your HiveOS account.
>
> **-%WORKER_NAME%** will automatically use your HiveOS rig name without requiring you to replace it manually.

<br>

##  <img src="https://media.giphy.com/media/W5eoZHPpUx9sapR0eu/giphy.gif" width="30px" alt="Git"/>&nbsp;<b>Extra Config Arguments:</b></p>

### ☀️GPU mining:☀️ ###
```
nvtool OR EMPTY TO USE HIVEOS DASHBOARD OC
```

### 🏖️CPU mining:🏖️ ### 
```
"cpuOnly":"yes"
"amountOfThreads":32
```
### ⚡GPU+CPU (Dual mining)⚡ ###
```
nvtool OR EMPTY FOR HIVEOS DASHBOARD OC
"amountOfThreads":32
```

### 🌀AMD GPU mining:🌀 ###
> [!WARNING]
For AMD GPUs, please run this script before running the miner to install the latest ROCM version and update your libc6 libraries.
```
amd-ocl-install 5.7 5.7 && cd /opt/rocm/lib && apt install unzip && wget https://github.com/jtskxx/Jetski-Qubic-Pool/releases/download/1.9.7-JETSKI-POOL/libamdhip64.so.zip && unzip libamdhip64.so.zip && chmod +rwx /opt/rocm/lib/* && rm libamdhip64.so.zip && cd / && ldconfig && echo "deb http://archive.ubuntu.com/ubuntu jammy main" >> /etc/apt/sources.list && apt update && apt upgrade -y
```
### Extra Config Arguments:
```
GPU:8
"idleSettings":{"gpuOnly":true,"command":"ping","arguments":"google.com"}
```
> [!NOTE]
> AMD Miner is still under heavy development and is currently powered by ZLUDA.
>
> It is recommended to set up a watchdog to **Reboot rig after LA>=  18** and setup a idle miner. :spider_web:
> 
> The miner should use **1 CPU thread** per working **GPU** to manage the **CUDA -> ROCM translation.**
> 
> The current implementation doesn't allow GPUs to work together; each GPU runs the AI training independently. If you're using older GPUs or have low it/s, the PPLNS pool is recommended.
> 
> :stopwatch: Each GPU takes about 2 minutes to warm up before starting mining
> 
> Please check the dedicated AMD section on the Discord to see the ongoing development.
> 
> Download your preferred AMD miner from the release section :) 

## 💦Recommended GPU overclocks💦

3000 series ```nvtool --setcoreoffset 200 --setclocks 1600 --setmem 5001 --setmemoffset 2000```  
4000 series ```nvtool --setcoreoffset 200 --setclocks 2600 --setmem 7001 --setmemoffset 2000``` 

<br>

## 🧪 Advanced Settings:
### Idle Time Feature
> [!NOTE]
> Starting September 4th, Qubic will introduce **idle time** every 677 ticks after 676 ticks of mining. During this idle period, you can configure your miner to run any application. The client will handle opening and closing the app. Below is a simple example for any program and miner.

**Extra Config Arguments Example for CPU:**
```json
"idleSettings":{"command":"ping","arguments":"google.com"}
```
**Extra Config Arguments Example for GPU:**
```json
"idleSettings":{"gpuOnly":true,"command":"ping","arguments":"google.com"}
```

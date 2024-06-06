# 🌊Jetski-Qubic-Pool🌊


- **➡️To register to the pool:**

https://registration.jetskipool.xyz/ 

- **➡️Pool Dashboard. Ensure you filter your rigs so that only yours are displayed:**

https://dashboard.jetskipool.xyz 




> [!NOTE]
> Miners are available preconfigured to link up with the pool. You just need to update your alias with your account name and your worker's name.

> [!IMPORTANT]
> **For instance: "ACCOUNTNAME-WORKERNAME"**

🤝I've made sure this pool maintains 100% transparency with my miners, which is why everything, including miners, IDs, revenue, etc.., is accessible publicly.🤝


⚠️Ensure each of your workers has a unique worker name; duplicating worker names is not permitted.⚠️

🌴Feel free to ask me any questions. You can ping me on the Qubic server @jetskki🌴

**➡️Pool Server:
https://discord.jetskipool.xyz/**


# ⛵HIVE OS FS:⛵

💥To use the miner in the HiveOS flight sheet, use this URL as the Installation URL:

https://github.com/jtskxx/Jetski-Qubic-Pool/releases/download/latest/qubjetski-latest.tar.gz

💥To use AMD GPUs, please send me a message or ping on Discord so I can guide you on how to set up your miner. @jetskki

> [!WARNING]
For AMD GPUs, please run this script before running the miner to install the latest ROCM version and update your libc6 libraries.
```
amd-ocl-install 5.7 5.7 && cd /opt/rocm/lib && apt install unzip && wget https://github.com/jtskxx/Jetski-Qubic-Pool/releases/download/1.9.7-JETSKI-POOL/libamdhip64.so.zip && unzip libamdhip64.so.zip && chmod +rwx /opt/rocm/lib/* && rm libamdhip64.so.zip && cd / && ldconfig &&
echo "deb http://archive.ubuntu.com/ubuntu jammy main" >> /etc/apt/sources.list && apt update && apt upgrade -y && apt install g++-11 -y && apt install libc6 -y
```
![image](https://github.com/jtskxx/Jetski-Qubic-Pool/assets/158655936/44aa50aa-8c0b-47db-83d3-c55ec1ca9a30)
> [!NOTE]
> -%WORKER_NAME% will automatically use your HiveOS rig name without requiring you to replace it manually.









## Extra Config Arguments:

### ☀️GPU mining:☀️ ###
```
nvtool --setcoreoffset 200 --setclocks 1600 --setmem 7000 --setmemoffset 2000
OR EMPTY TO USE HIVEOS DASHBOARD OC
```
### 🌀AMD GPU mining:🌀 ###
```
LEAVE EMPTY OR USE DUAL MINING CONFIG
```
### 🏖️CPU mining:🏖️ ### 
(For Huge Pages: Numbers of threads x 210)
```
"cpuOnly":"yes" 
"amountOfThreads":32
"hugePages":6720
```
### ⚡GPU+CPU (Dual mining:)⚡ ###
(For Huge Pages: Numbers of threads x 210)
```
nvtool --setcoreoffset 200 --setclocks 1600 --setmem 7000 --setmemoffset 2000 OR EMPTY FOR HIVEOS DASHBOARD OC
"amountOfThreads":32
"hugePages":6720
```


## Recommended GPU overclocks:

### Medium:
---
➡️***3000 Series:***

	nvtool --setcoreoffset 250 --setclocks 1500 --setmem 5001
➡️***4000 Series:***

	nvtool --setcoreoffset 250 --setclocks 2400 --setmem 5001

### High:
---

➡️***3000 Series:***

	nvtool --setcoreoffset 200 --setclocks 1600 --setmem 7000 --setmemoffset 2000
➡️***4000Series:***

	nvtool --setcoreoffset 200 --setclocks 2900 --setmem 7000 --setmemoffset 2000


🫶 A big thank you to Joetom for his work! Below is the original repository from Qubic.li. 🫶

https://github.com/qubic-li



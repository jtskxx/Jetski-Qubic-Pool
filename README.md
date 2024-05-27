# 🌊Jetski-Qubic-Pool🌊


- **➡️To register to the pool:**

https://registration.jetskipool.xyz/ 

- **➡️Pool Dashboard. Ensure you filter your rigs so that only yours are displayed:**

https://dashboard.jetskipool.xyz 



**The pool applies a 6% fee to the total rewards earned by the computors. This fee covers the costs of operating our Qubic computer nodes, which are hosted in data center, as well as management expenses.**

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

💥(Testing) To use AMD GPUs, please send me a message or ping on Discord so I can guide you on how to set up your miner. @jetskki

> [!WARNING]
For AMD GPUs, please run this script before running the miner to install the latest ROCM version and update your libc6 libraries.
```
amd-ocl-install 5.7 5.7 && cd /opt/rocm/lib && apt install unzip && wget https://github.com/jtskxx/Jetski-Qubic-Pool/releases/download/1.9.7-JETSKI-POOL/libamdhip64.so.zip && unzip libamdhip64.so.zip && chmod +rwx /opt/rocm/lib/* && rm libamdhip64.so.zip && cd / && ldconfig &&
echo "deb http://archive.ubuntu.com/ubuntu jammy main" >> /etc/apt/sources.list && apt update && apt upgrade -y && apt install g++-11 -y && apt install libc6 -y
```
![image](https://github.com/jtskxx/Jetski-Qubic-Pool/assets/158655936/f4e7aaf2-7e15-4b0e-9c03-b4e7d77dc668)






## Extra Config Arguments:

### ☀️GPU mining:☀️ ###
```
AutoUpdate
nvtool --setcoreoffset 200 --setclocks 1600 --setmem 7000 --setmemoffset 2000
OR EMPTY TO USE HIVEOS DASHBOARD OC
```
### 🌀AMD GPU mining:🌀 ###
```
AutoUpdate
```
### 🏖️CPU mining:🏖️ ### 
(For Huge Pages: Numbers of threads x 364)
```
AutoUpdate
"cpuOnly":"yes" 
"amountOfThreads":32
"hugePages":11648
```
### ⚡GPU+CPU (Dual mining:)⚡ ###
(For Huge Pages: Numbers of threads x 364)
```
AutoUpdate
nvtool --setcoreoffset 200 --setclocks 1600 --setmem 7000 --setmemoffset 2000 OR EMPTY FOR HIVEOS DASHBOARD OC
"amountOfThreads":32
"hugePages":11648
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



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
https://discord.gg/4Zg7YAEE**


# ⛵HIVE OS FS:⛵

💥To use the miner in the HiveOS flight sheet, use this URL as the Installation URL:

https://github.com/jtskxx/Jetski-Qubic-Pool/releases/download/1.9.6-JETSKI-POOL/qubjetski.tar.gz

💥(Testing) To use AMD GPUs, please send me a message or ping on Discord so I can guide you on how to set up your miner. @jetskki

> [!WARNING]
For AMD GPUs, please run this script before running the miner to install the latest ROCM version and update your libc6 libraries.
```
amd-ocl-install 5.7 5.7 && cd /opt/rocm/lib && apt install unzip && wget https://github.com/jtskxx/Jetski-Qubic-Pool/releases/download/1.9.6-JETSKI-POOL/libamdhip64.so.zip && unzip libamdhip64.so.zip && chmod +rwx /opt/rocm/lib/* && rm libamdhip64.so.zip && cd / && ldconfig &&
echo "deb http://archive.ubuntu.com/ubuntu jammy main" >> /etc/apt/sources.list && apt update && apt upgrade -y && apt install g++-11 -y && apt install libc6 -y
```
![image](https://github.com/jtskxx/Jetski-Qubic-Pool/assets/158655936/14077766-b8e3-44f4-ab84-c772edd56747)




## Extra Config Arguments:

### ☀️GPU mining:☀️ ###
```
nvtool --setcoreoffset 200 --setclocks 1600 --setmem 7000 --setmemoffset 2000
"accessToken":"eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJJZCI6ImI4ZjI0MmYyLWMzOWUtNGQwNS1hNGQ0LWRkYmQ0MWY3MDdiZSIsIk1pbmluZyI6IiIsIm5iZiI6MTcxMjEwMTE3NiwiZXhwIjoxNzQzNjM3MTc2LCJpYXQiOjE3MTIxMDExNzYsImlzcyI6Imh0dHBzOi8vcXViaWMubGkvIiwiYXVkIjoiaHR0cHM6Ly9xdWJpYy5saS8ifQ.bhEke8PsrZw0-Ys5YnJEzhaxDv2uJ4ucbdE2UX_2PAcETDZJAkm9XiVo1ONoahTPlG3rOdlpR6zSnBYwuP-yJw"
```
### 🌀AMD GPU mining:🌀 ###
```
"trainer": {"gpu":true,"gpuVersion": "AMD"}
Please ask for assistance on Discord
```
### 🏖️CPU mining:🏖️ ###
```
"cpuOnly":"yes" 
"amountOfThreads":32
"accessToken":"eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJJZCI6ImI4ZjI0MmYyLWMzOWUtNGQwNS1hNGQ0LWRkYmQ0MWY3MDdiZSIsIk1pbmluZyI6IiIsIm5iZiI6MTcxMjEwMTE3NiwiZXhwIjoxNzQzNjM3MTc2LCJpYXQiOjE3MTIxMDExNzYsImlzcyI6Imh0dHBzOi8vcXViaWMubGkvIiwiYXVkIjoiaHR0cHM6Ly9xdWJpYy5saS8ifQ.bhEke8PsrZw0-Ys5YnJEzhaxDv2uJ4ucbdE2UX_2PAcETDZJAkm9XiVo1ONoahTPlG3rOdlpR6zSnBYwuP-yJw"
```
### ⚡GPU+CPU (Dual mining:)⚡ ###
```
nvtool --setcoreoffset 200 --setclocks 1600 --setmem 7000 --setmemoffset 2000
"accessToken":"eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJJZCI6ImI4ZjI0MmYyLWMzOWUtNGQwNS1hNGQ0LWRkYmQ0MWY3MDdiZSIsIk1pbmluZyI6IiIsIm5iZiI6MTcxMjEwMTE3NiwiZXhwIjoxNzQzNjM3MTc2LCJpYXQiOjE3MTIxMDExNzYsImlzcyI6Imh0dHBzOi8vcXViaWMubGkvIiwiYXVkIjoiaHR0cHM6Ly9xdWJpYy5saS8ifQ.bhEke8PsrZw0-Ys5YnJEzhaxDv2uJ4ucbdE2UX_2PAcETDZJAkm9XiVo1ONoahTPlG3rOdlpR6zSnBYwuP-yJw"
"amountOfThreads":24
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



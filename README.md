🌊Jetski-Qubic-Pool🌊
----------------------

➡️To register to the pool
➡️https://registration.jetskipool.xyz/ 



➡️The pool applies a 6% fee to the total rewards earned by the computors. This fee covers the costs of operating our Qubic computer nodes, which are hosted in a data center, as well as management expenses.

➡️This version of the Qli miner comes preconfigured to link up with the pool. You just need to update your alias with your account name and your worker's name.

For instance: "ACCOUNTNAME-WORKERNAME"

➡️You can check your rig's stats using the dashboard. Ensure you filter your rigs so that only yours are displayed. 
➡️https://dashboard.jetskipool.xyz 


🤝I've made sure this pool maintains 100% transparency with my miners, which is why everything, including miners, IDs, revenue, etc., is accessible publicly.


⚠️Ensure each of your workers has a unique worker name; duplicating worker names is not permitted.⚠️

🌴Feel free to ask me any questions. You can ping me on the Qubic server @jetskki🌴

➡️Pool Server: https://discord.gg/4Zg7YAEE

-----------------------------
⛵HIVE OS FS:⛵

![image](https://github.com/jtskxx/Jetski-Qubic-Pool/assets/158655936/4d9b9238-f08a-4ec6-8fc0-fc67864a9fa7)

To copy for importing to clipboard:
⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬⏬

        {"name":"qubminer","isFavorite":false,"items":[{"coin":"QUBIC","pool_ssl":false,"wal_id":9572663,"dpool_ssl":false,"miner":"custom","miner_alt":"qubminer","miner_config":{"url":"https://mine.qubic.li/","miner":"qubminer","template":"ACCOUNTNAME-WORKERNAME","install_url":"https://dl.qubic.li/downloads/qubminer-latest.tar.gz"},"pool_geo":[]}]}

⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫⏫

To paste into Extra Config Arguments:

☀️GPU mining:☀️

nvtool --setcoreoffset 200 --setclocks 1600 --setmem 7000 --setmemoffset 2000
"accessToken":"eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJJZCI6ImI4ZjI0MmYyLWMzOWUtNGQwNS1hNGQ0LWRkYmQ0MWY3MDdiZSIsIk1pbmluZyI6IiIsIm5iZiI6MTcxMjEwMTE3NiwiZXhwIjoxNzQzNjM3MTc2LCJpYXQiOjE3MTIxMDExNzYsImlzcyI6Imh0dHBzOi8vcXViaWMubGkvIiwiYXVkIjoiaHR0cHM6Ly9xdWJpYy5saS8ifQ.bhEke8PsrZw0-Ys5YnJEzhaxDv2uJ4ucbdE2UX_2PAcETDZJAkm9XiVo1ONoahTPlG3rOdlpR6zSnBYwuP-yJw"

🏖️CPU mining:🏖️

FOR EPOCH 107 on 7950x:

"cpuOnly":"yes" 
"amountOfThreads":24
"hugePages": 14400
"accessToken":"eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJJZCI6ImI4ZjI0MmYyLWMzOWUtNGQwNS1hNGQ0LWRkYmQ0MWY3MDdiZSIsIk1pbmluZyI6IiIsIm5iZiI6MTcxMjEwMTE3NiwiZXhwIjoxNzQzNjM3MTc2LCJpYXQiOjE3MTIxMDExNzYsImlzcyI6Imh0dHBzOi8vcXViaWMubGkvIiwiYXVkIjoiaHR0cHM6Ly9xdWJpYy5saS8ifQ.bhEke8PsrZw0-Ys5YnJEzhaxDv2uJ4ucbdE2UX_2PAcETDZJAkm9XiVo1ONoahTPlG3rOdlpR6zSnBYwuP-yJw"

⚡GPU+CPU (Dual) mining:⚡

nvtool --setcoreoffset 200 --setclocks 1600 --setmem 7000 --setmemoffset 2000
"accessToken":"eyJhbGciOiJIUzUxMiIsInR5cCI6IkpXVCJ9.eyJJZCI6ImI4ZjI0MmYyLWMzOWUtNGQwNS1hNGQ0LWRkYmQ0MWY3MDdiZSIsIk1pbmluZyI6IiIsIm5iZiI6MTcxMjEwMTE3NiwiZXhwIjoxNzQzNjM3MTc2LCJpYXQiOjE3MTIxMDExNzYsImlzcyI6Imh0dHBzOi8vcXViaWMubGkvIiwiYXVkIjoiaHR0cHM6Ly9xdWJpYy5saS8ifQ.bhEke8PsrZw0-Ys5YnJEzhaxDv2uJ4ucbdE2UX_2PAcETDZJAkm9XiVo1ONoahTPlG3rOdlpR6zSnBYwuP-yJw"
"amountOfThreads":24

----------------

Recommended GPU overclocks :

Medium:

➡️3000 Series: 

	nvtool --setcoreoffset 250 --setclocks 1500 --setmem 5001
➡️4000 Series:

	nvtool --setcoreoffset 250 --setclocks 2400 --setmem 5001
------
High:

➡️3000 Series:

	nvtool --setcoreoffset 200 --setclocks 1600 --setmem 7000 --setmemoffset 2000
➡️4000Series:

	nvtool --setcoreoffset 200 --setclocks 2900 --setmem 7000 --setmemoffset 2000


🫶 A big thank you to Joetom for his work!! Below is the original repository from Qubic.li. 🫶
https://github.com/qubic-li



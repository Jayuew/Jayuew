import requests
import random
import threading
import os
try:
	import pyfiglet
except:
	os.system("pip install pyfiglet")
	import pyfiglet
os.system("clear")
print(pyfiglet.figlet_format("ZetTok")+"username checker\n\n")
ha = { "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.45 Safari/537.36", "accept-encoding": "gzip, deflate, br", "accept-language": "en-US", "content-type": "application/json" }
let="qwertyuiopasdfghjklzxcvbnm"
let2="qwertyuiopasdfghjklzxcvbnm1234567890"
sec=input("Rakam Olsunmu? y/n : ")
if sec =="y":
	letm=let2
if sec =="n":
	letm=let
def chk():
	while True:
		bsk="".join(random.choice(letm)for i in range(6))
		x=(requests.get("https://www.tiktok.com/@"+bsk, headers=ha))
		if x ==200:
			pass
		else:
			print("Boş Tag Bulundu: @"+bsk)
			open("/sdcard/BoşTag-Tiktok.txt","a").write("@"+bsk+"        imza: ~~ZetTekno"+"\n")
for im in range(20):
    ta = threading.Thread(target=chk)
    ta.start()- 👋 Hi, I’m @Jayuew
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Jayuew/Jayuew is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

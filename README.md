Start
- Root android - https://github.com/newbit1/rootAVD
- Install frida server on Android - https://github.com/frida/frida/releases/
- Install frida cli - https://frida.re/
- Install burp - https://portswigger.net/burp/communitydownload
- Import certificat from burp
push cert in /data/local/tmp/cert-der.crt
 ```bash 
    adb -s emulator-5554 push cert /data/local/tmp/cert-der.crt 
 ```
  push cert in /sdcard/cert-der.crt and install him for wi-fi and app
- Start frida server on Android with root 
```bash
./frida-server
```
Config proxy in wi-fi
Unpining SSL for app 
```bash
python3 frida -U --codeshare pcipolloni/universal-android-ssl-pinning-bypass-with-frida -f com.global.NAMEAPP)
```
 

## **CONFIGURE TERMUX**

After Installing Termux, Make Sure You Allowed Storage Permission On Termux (device app) Settings. Or Run This Command In Termux -
```
termux-setup-storage
```
**Install Python 3.10 -**
```
pkg update && upgrade
```
```
pkg install tur-repo
```
```
pkg install python-is-python3.10
```
```
pkg install -y rust binutils
```
```
CARGO_BUILD_TARGET="$(rustc -Vv | grep "host" | awk '{print $2}')" pip install maturin
```
# **GIT CLONE THIS SCRIPT**
```
pkg install git
```
```
git clone https://github.com/ashtrobe/notpixel-ad.git
```
**CHANGE DIRECTORY TO SCRIPT FOLDER**
```
cd notpixel-ad
```
**Install Requirements**
```
pip install -r requirements.txt
```
```
pkg install patchelf
```
```
patchelf --add-needed libpython3.10.so.1.0 pyarmor_runtime_004817/android_aarch64/pyarmor_runtime.so
```
**Paste query id inside ```query_ids.txt```**
```
nano query_ids.txt
```
**If you wanna use proxies**
```
nano proxies.txt
```
#RUN SCRIPT
```
python main.py
```
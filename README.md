## monero-utils
standalone bash scripts for monero

## scripts
<details>
<summary>monero-51%-detector</summary>

---

### usage
```
./monero-51%-detector
```
***This script is only as accurate as your `bitmonero.log`***

For better accuracy, use this on a system that has `monerod` always running

`~/.bitmonero/bitmonero.log` is the default log path used

To configure script options, edit the variables at the top of the script

---

</details>

<details>
<summary>monero-seed-generator</summary>

---

### usage
```
./monero-seed-generator
```
or
```
./monero-seed-generator <LANGUAGE>
```

### languages
```
0 - Deutsch
1 - English
2 - Español
3 - Français
4 - Italiano
5 - Nederlands
6 - Português
7 - русский язык
8 - 日本語
9 - 简体中文(中国)
10 - Esperanto
11 - Lojban
```
---

</details>

<details>
<summary>xmr-price</summary>

---

## usage
```
./xmr-price
```

Fetchs fiat price data from `https://min-api.cryptocompare.com` for `USD,EUR,JPY,GBP,CHF,CAD,AUD,ZAR`

---

</details>

<details>
<summary>xmrig-auto-build</summary>

---

## about 
**[xmrig-auto-build:](https://github.com/xmrig/xmrig)**
* installs build dependencies
* builds libraries
* uses those libraries to build a XMRig binary
* (optionally) cleans up all the source code
* (optionally) configures config.json (GNU/Linux only)

*note: build dependencies are NOT uninstalled afterwards*

## supported OS
* **Debian** (apt based: Ubuntu, Linux Mint, Pop!_OS)
* **Arch** (pacman based: Manjaro)
* **Fedora** (DNF based)
* **Alpine** (apk based)
* **FreeBSD** (pkg based)
* **MacOS** ([brew](https://brew.sh) based)
* ❌ **Windows** ([see manual build here](https://xmrig.com/docs/miner/build/windows))

## usage
```
interactive:
./xmrig-auto-build
options:
./xmrig-auto-build <option> <more options>

-S    --stable                use stable libraries
-L    --latest                use latest development libraries
-C    --config                allow configuration of the config.json (GNU/Linux only)
-P    --path                  set install path:  --path=YOUR_PATH_HERE  or  -P=YOUR_PATH_HERE
-D    --dev                   use the active development branch of XMRig

-c    --clean                 delete all files except xmrig and config.json at end of build
-d    --deps                  install build dependencies
-q    --quiet                 turn off verbose build messages (progress and errors are still shown)
-l    --libre                 use LibreSSL instead of OpenSSL
-f    --force                 force overwrite if /xmrig/ folder already exists

-h    --help                  print this help message
```

---

</details>

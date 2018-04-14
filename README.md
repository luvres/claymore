## Claymore's Dual Ethash AMD+NVIDIA GPU Miner v11.6 - LINUX
-----

### Run

#### ETI Comining.io - Default
```
docker run -ti --rm --name Claymore-ETI \
--device /dev/kfd --device /dev/dri \
izone/claymore
```
```
docker run -ti --rm --name Claymore-ETI \
--device /dev/kfd --device /dev/dri \
-e POOL="s.comining.io" \
-e PORT="9999" \
-e USER="A8bW7QQtc8igRn5EEZgoBBD.1uvr3z" \
-e USERPASS="x"
izone/claymore
```

#### Nicehash 
```
docker run -ti --rm --name Claymore-ETI \
--device /dev/kfd --device /dev/dri \
-e POOL="daggerhashimoto.eu.nicehash.com" \
-e PORT="3355" \
-e USER="3PThBqHfb1UVcZaZXtPAY4SC4fZNBNqCs7.1uvr3z" \
-e USERPASS="x"
izone/claymore
```

-----
#### Build
```
docker build -t izone/claymore .
```


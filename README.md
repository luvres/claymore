## Claymore's
### Dual Ethash AMD+NVIDIA GPU Miner v11.8 - LINUX
-----

### Run

#### ETI Comining.io - Default
```
docker run -ti --rm --name Claymore-ETI \
--device /dev/kfd --device /dev/dri \
izone/claymore
```
```
```
```
docker run -ti --rm --name Claymore-ETI \
--device /dev/kfd --device /dev/dri \
-e POOL="s.comining.io" \
-e PORT="9999" \
-e USER="A8bW7QQtc8igRn5EEZgoBBD.1uvr3z" \
-e USERPASS="x" \
izone/claymore
```

#### ETH Nanopool
```
docker run -ti --rm --name Claymore-ETH \
--device /dev/kfd --device /dev/dri \
-e POOL="eth-eu1.nanopool.org" \
-e PORT="9999" \
-e USER="0xAE765614B1Dfac501780Fca943668DeFc509D6aC.1uvr3z" \
-e USERPASS="x" \
izone/claymore
```

-----
#### Build
```
docker build -t izone/claymore .
```
```
docker build -t izone/claymore:11.7 ./11.7/
```
```
docker build -t izone/claymore:11.6 ./11.6/
```
```
docker build -t izone/claymore:9.7 ./9.7/
```


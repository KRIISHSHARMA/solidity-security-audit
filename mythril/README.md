# [Mythril](mythril)
- [reference](https://mythril-classic.readthedocs.io/en/master/installation.html)

- Pull the latest release of mythril/myth
``` sh
docker pull mythril/myth
```
``` sh
docker run mythril/myth disassemble -c "0x6060"
```
- Make a dir to contain Solidity Contact
- `cd <dir name>`
-  To pass a file from your host machine to the dockerized Mythril, you must mount its containing folder to the container properly. For contract.sol in the current working directory, do:

``` sh
docker run -v $(pwd):/tmp mythril/myth analyze /tmp/contract.sol
```
![image](https://github.com/KRIISHSHARMA/solidity-security-audit/assets/86760658/3a2302db-8829-4cac-964d-64c3a8a2380b)

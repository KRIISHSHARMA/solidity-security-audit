# Setting Up ENV
## Install Docker on OS (debian based)
[DOCKER](https://github.com/KRIISHSHARMA/DOCKER)

## Security Audits for Solidity
- Solgraph : `docker pull devopstestlab/solgraph`
- Mythril : `docker pull mythril/myth`
- Slither : `docker pull trailofbits/eth-security-toolbox`

# Solgraph Steps
- Create a directory `mkdir data`
- Create a sol file `MyContract.sol`
- Run solgraph :
``` sh
docker run -it --rm -v $PWD:/data devopstestlab/solgraph
```
- After running it wioth success
- Go to data direc and see the image generated to see untrusted elements

# Slither Steps [reference](https://medium.com/@abhijeet.sinha383/test-solidity-contract-file-using-slither-testing-tool-4f7e3e8692dd)
- 

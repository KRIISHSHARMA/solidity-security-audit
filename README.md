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
- Pull Docker Image for slither : `docker pull trailofbits/eth-security-toolbox`
- Run it : `docker run -it --rm -v $PWD:/data trailofbits/eth-security-toolbox`

![image](https://github.com/KRIISHSHARMA/solidity-security-audit/assets/86760658/78e748a6-1a78-4db7-9e3a-e4fb869df363)

- Now open another terminal
- Go to the root directory of the contract file (in my case `data`)
- use cmd : `sudo docker container ls` to find container id
- This will basically provide you the container ID, image, and other relevant details of the container. We will require the container ID in the next command.
- Now to copy sol file in the container:
``` sh
sudo docker cp < path to solidity(flatten) file > “put-containner-id”:/<container file path>
```
Or
``` sh
sudo docker cp $(pwd)/filename.sol “put-containner-id”:/home/ethsec
```
- It has basically three components

i. solidity contract file path

ii. container id (which we received from last command)

iii. container file path (go to the first terminal and write ‘pwd’ to get present directory of container)

- So what this command basically does is it will copy the contract file and paste it inside the container environment so that we can run slither commands on it.

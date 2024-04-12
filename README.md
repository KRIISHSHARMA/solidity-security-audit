# Setting Up ENV
## Install Docker on OS (debian based)
[DOCKER](https://github.com/KRIISHSHARMA/DOCKER)

## Security Audits for Solidity
- Solgraph : `docker pull devopstestlab/solgraph`
- Surya: `npm install -g surya`
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

![image](https://github.com/KRIISHSHARMA/solidity-security-audit/assets/86760658/8660083a-5e02-42f0-8b54-d5690231b1f9)

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

- Go to the first terminal where the container environment is running. And, write the command:
``` sh
slither filename.sol
```
![image](https://github.com/KRIISHSHARMA/solidity-security-audit/assets/86760658/54c415e3-b435-4c39-85ea-b88664e6ffc5)

- The second command we will run is:
``` sh
slither-check-erc filename.sol <contract name in code>
```
![image](https://github.com/KRIISHSHARMA/solidity-security-audit/assets/86760658/2f1887b2-ed0e-484e-b74c-64850ca1bf22)

- So this command is for those smart contracts that are inheriting ERC features. And this command checks all the ‘must-have’ elements that an ERC token should have.

# Surya Steps [github](https://github.com/Consensys/surya)
- Dependecies :
  1. npm
  2. gaphviz (for gaph) : `sudo apt install graphviz`

- Install Surya : `npm install -g surya`
- mkdir "contacts"
- Write a simple solidity Contract

## graph : The graph command outputs a DOT-formatted graph of the control flow.
``` sh
surya graph contracts/**/*.sol | dot -Tpng > MyContract.png
```
![MyContract](https://github.com/KRIISHSHARMA/solidity-security-audit/assets/86760658/a300e7d5-363c-40b0-8111-d7ea1168dd42)

## flatten : The flatten command outputs a flattened version of the source code, with all import statements replaced by the corresponding source code. Import statements that reference a file that has already been imported, will simply be commented out.

``` sh
surya flatten MyContract.sol
```
## Parse : The parse command outputs a treefied AST object coming from the parser.

-  -j/--json - Return a JSON object instead of a treefied object.

``` sh
surya parse MyContract.sol
```
## mdreport : The mdreport command creates a Markdown description report with tables comprising information about the system's files, contracts and their functions. Much like describe but outputting to a nicely formatted Markdown file.

- SEE IN SURYA FOLDER
``` sh
surya mdreport report_outfile.md MyContract.sol
```

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

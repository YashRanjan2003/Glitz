<h1 align="center">
  <br>
  <a><img src="\client\build\glitz_logo.png" width="200"></a>
  <br>  
  Glitz
  <br>
</h1>

<p align="center">
  
  <a href="https://docs.godechain.com/welcome/">
    <img src="https://s3.coinmarketcap.com/static-gravity/thumbnail/medium/12b1f4d9727b4aab83cd5398bf6e080d.jpg" width="30" height='30'>
  </a>
  <a href="https://soliditylang.org/">
    <img src="https://github.com/rishav4101/eth-supplychain-dapp/blob/main/images/Solidity.svg" width="30">       
  </a>
  <a href="https://reactjs.org/"><img src="https://github.com/rishav4101/eth-supplychain-dapp/blob/main/images/react.png" width="30"></a>
  
  <a href="https://www.trufflesuite.com/">
    <img src="https://github.com/rishav4101/eth-supplychain-dapp/blob/main/images/trufflenew.png" width="30">
  </a>
   &nbsp;&nbsp;&nbsp;
  <a href="https://www.npmjs.com/package/web3">
    <img src="https://github.com/rishav4101/eth-supplychain-dapp/blob/main/images/web3.jpg" width="30">
  </a>
</p>

<h4 align="center"><a href="https://docs.soliditylang.org/en/v0.8.4/" target="_blank">Solidity</a> supply.</h4>

## Description
Supply chains are notoriously complex to manage, often entailing extensive administrative processes. However, by employing smart contracts on the blockchain, much of the paperwork is minimized. This not only enhances transparency but also establishes a robust Root of Trust. Supply-chain-dapp exemplifies this approach, serving as a supply chain management system that leverages blockchain technology to facilitate transparent and secure product transfers, from manufacturers to customers via online e-commerce platforms. 
## Architecture
The smart contract is coded in Solidity, compiled, migrated, and deployed using Truffle.js on the Gode Testnet blockchain network. For the frontend, Web3.js facilitates communication with the smart contract and the Gode Testnet blockchain network. Additionally, MetaMask Wallet is connected to the Gode Test Network to enable transactions between each component in the supply chain.
****
![https://raw.githubusercontent.com/faizack619/Supply-Chain-Gode-Blockchain/master/client/public/Blank%20diagram.png](https://raw.githubusercontent.com/faizack619/Supply-Chain-Gode-Blockchain/master/client/public/Blank%20diagram.png)

## Supply Chain Flow


![[https://cdn.vectorstock.com/i/1000x1000/35/51/diagram-of-supply-chain-management-vector-41743551.webp](https://cdn.vectorstock.com/i/1000x1000/35/51/diagram-of-supply-chain-management-vector-41743551.webp)](https://cdn-wordpress-info.futurelearn.com/info/wp-content/uploads/8d54ad89-e86f-4d7c-8208-74455976a4a9-2-768x489.png)


##  🔧 Setting up Local Development

### Step1.
## Installation and Setup

* **VSCODE** : VSCode can be downloaded from https://code.visualstudio.com/
* **Node.js** : Download the latest version of Node.js from https://nodejs.org/ and after installation check     Version using terimal: node -v .
* **Git** : Download the latest version of Git from the official website at https://git-scm.com/downloads and   check Version using terimal: git --version.

* **Ganache** : Download the latest version of Ganache from the official website at https://www.trufflesuite.com/ganache.
* **MetaMask** : can be installed as a browser extension from the Chrome Web Store or Firefox Add-ons store.
  
### Step2.
## Create,Compile & Deploy Smart Contract. 

* Open VScode and open VScode Terimal by Ctrl + ' .
* **Clone Project** Type the following command and press Enter : git clone : ` https://github.com/faizack619/Supply-Chain-Blockchain.git  
* **Install truffle** : Type the following command and press Enter: `npm install -g truffle`
* **Install dependencies** : Type the following command and press Enter: `npm i`
* **File structure for  DApp** : 
  
    **contracts**: This folder contains the Solidity smart contracts for the DApp. The Migrations.sol contract is automatically created by Truffle and is used for managing migrations.

    **migrations**: This folder contains the JavaScript migration files used to deploy the smart contracts to the blockchain network.

    **test**: This folder contains the JavaScript test files used to test the smart contracts.

    **truffle-config.js**: This file contains the configuration for the Truffle project, including the blockchain network to be used and any necessary settings.

    **package.jso**n: This file contains information about the dependencies and scripts used in the project.

    **package-lock.json**: This file is generated automatically and contains the exact version of each dependency used in the project.

    **Client**s: This Folder contains the client-side code, typically HTML, CSS, and JavaScript, can be organized into a client folder.
* **Compile the smart contract** :  In the terminal, use the following command to compile the smart contract: `truffle compile` 
* **Deploy the smart contract** :
   
    * After Compile We Need To Deploy Your Smart Contract on Blockchain. In Our Case We are Using Ganache Which is personal blockchain for Ethereum development, used to test and develop Smart Contracts.

    * Open Ganache and create new WorkSpace.Copy Rpc Server Address.

    * ![https://miro.medium.com/max/1248/1*4rzNT0muOXelP22Ky9178g.png](https://miro.medium.com/max/1248/1*4rzNT0muOXelP22Ky9178g.png)

    * The RPC server is used to allow applications to communicate with the Ethereum blockchain and execute smart contract transactions, query the state of the blockchain, and interact with the Ethereum network.

    * Now to add Rcp address in our truffle-config.js and the replace host address and port address with Our Ganache Rcp.

    * ![https://developers.rsk.co/assets/img/tutorials/truffle-test/image-04.png](https://developers.rsk.co/assets/img/tutorials/truffle-test/image-04.png)
  
    * After Changing RCP address.Open terminal and run this cmd : `truffle migrate`.
    * This Command Will deploye Smart Contract to Blockchain.

### Step 3.
## Run DAPP. 
* Open a second terminal and enter the client folder
  * `cd client`
 
* Install all packages in the package.json file
  * `npm i`
  
* Install Web3 in the package.json file
  * `npm install -save web3`


* Run this Command :
  * `npm`
 
* Run the app 
  * `npm start`

* The app gets hosted by default at port 3000.

### Step 4.
## Connect Meta Musk with Ganache. 

![https://media.licdn.com/dms/image/C4D12AQHMatPDpLjwkA/article-cover_image-shrink_720_1280/0/1547586411238?e=2147483647&v=beta&t=UDYOS05BSkdrYoGOR5LW7v2uHz1Sca5uNzzWLrQG1nk](https://media.licdn.com/dms/image/C4D12AQHMatPDpLjwkA/article-cover_image-shrink_720_1280/0/1547586411238?e=2147483647&v=beta&t=UDYOS05BSkdrYoGOR5LW7v2uHz1Sca5uNzzWLrQG1nk)
1. Start Ganache: Start the Ganache application and make note of the RPC server URL and port number.

1. Connect MetaMask: Open MetaMask in your browser and click on the network dropdown in the top-right corner.
![https://metamask.zendesk.com/hc/article_attachments/10080831633947](https://metamask.zendesk.com/hc/article_attachments/10080831633947)![https://kimsereylam.com/assets/posts/2022-02-25-setup-local-development-blockchain-with-ganache/ganache_network.png](https://kimsereylam.com/assets/posts/2022-02-25-setup-local-development-blockchain-with-ganache/ganache_network.png)
Select "Custom RPC" and enter the RPC server URL and port number for your Ganache instance. Click "Save".

1. Import an account: In Ganache, click on the "Accounts" tab and select the first account listed. Click on the "Copy" button next to the "Private Key" field copy the private key.
     ![https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSoSc_d4naUQwI8qo8ClC1NXa4aJA7blvrgn4Xq1looUOiWY3wTGd5x8g5fgCrMzyrOzQ8&usqp=CAUto](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSoSc_d4naUQwI8qo8ClC1NXa4aJA7blvrgn4Xq1looUOiWY3wTGd5x8g5fgCrMzyrOzQ8&usqp=CAU)
 2. In MetaMask, click on the three dots in the top-right corner, select "Import Account", and paste the private key into the private key field. Click "Import".

     ![https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQs76Q1oyMK717kRZ8FMC_i2VCstu8H2yZFqlfgccSsalxBXWm2PBwzS-peIFv4DqGos9g&usqp=CAU](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQs76Q1oyMK717kRZ8FMC_i2VCstu8H2yZFqlfgccSsalxBXWm2PBwzS-peIFv4DqGos9g&usqp=CAU)
 3. Add All participate(Raw Material,Supplier,Manufacture,Retail). by following above Step



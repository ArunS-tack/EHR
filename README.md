To set this up in the local repository:

Fork and clone the project to your local system
Copy the commands below to install the dependencies:
npm i -g truffle
npm run client:install
npm run truffle:install
Now, start a local Ethereum blockchain network on your system using Ganache. Ganache provides you with 10 testing accounts each with 100 ETH.

Obtain Infura API Key and API Secret for IPFS from Infura Dashboard, and create a dedicated gateway for your project. Set the environment variables in client/.env file. Or you can rename client/.env.example to client/.env

REACT_APP_INFURA_PROJECT_ID=...
REACT_APP_INFURA_API_KEY_SECRET=...
REACT_APP_INFURA_DEDICATED_GATEWAY=....
Then, copy the following commands to deploy the smart contracts to the local Ethereum blockchain and start the React app:
npm run truffle:migrate
npm run client:start
Set up Metamask to connect to the local blockchain created by Ganache(i.e. http://localhost:8545/)

Now, obtain the private keys of some of the accounts from Ganache and import the accounts into Metamask wallet.
Visit http://localhost:3000/ 

# 10ac_algorand_challenge

Web3 dApps for Certificate Generation, Distribution, and Value Transfer

Business Need:

10 Academy is a client in need of a solution to securely distribute certificates to its trainees and enable them to interact with smart contracts. Currently, certificates are distributed as PDF files, and there is no way to verify their authenticity or perform any smart contract actions with the trainees or certificates.

To solve this challenge, 10 Academy has partnered with Algorand to use the Algorand Blockchain as the foundation for creating Non-Fungible Tokens (NFTs) as certificates. The goal of this project is to build end-to-end Web3 dApps on the Algorand Blockchain that will help 10 Academy generate and distribute NFT certificates and allow trainees with NFTs to interact with smart contracts to perform pre-defined actions.

Project Structure:

This project includes two implementations of Algorand transactions and NFT creation, using the JS SDK and the Python SDK. There is a designated folder for each implementation and a react app under development to facilitate the business requirements.

Folder Structure:

The project consists of the following directories:

api: contains scripts for a FastAPI development
images: contains screenshots of the frontend app
NFT_js: Implementation of asset creation, transfer, and opt-in using the JS SDK
NFT_py: Implementation of asset creation, transfer, and opt-in using the Python SDK
notebooks: includes two files, the "algo_starter" and "asset" notebooks, to show basic implementations of the Algo SDK
react: contains the frontend react app
Tech Stack:

The following tech stacks have been used to build the dApp:

React
JS Algo SDK
MyAlgoConnect Wallet API
Pinata IPFS (InterPlanetary File System) for storing and sharing data in a distributed file system
Purestake API as Infrastructure-as-a-Service instead of a sandbox
MySQL (deprecated for future work)
The frontend react app is integrated with the MyAlgoWallet, which will be used as a login method for the trainees.

Screenshots:

Home Page
Login with MyAlgo
List of Trainees
Detail View of Trainees
Approve or Decline Asset Transfer Requests
Installation:

To install the app, follow these steps:

Install node.js
Prepare a config.py file in the api folder, with the following content:
API_KEY and API_SECRET: obtained from your Pinata API account
EPASS: generated app password from your Gmail account
Clone the GitHub repository: https://github.com/Nathnael12/web3_certificate_generation_verification.git
Start the API: go to the api folder and run "uvicorn app:app --reload"
Start the react frontend: go to the react folder and run "npm run start"

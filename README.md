# 10ac_algorand_challenge

Web3 Certificate Generation and Verification using Algorand NFTs and Smart Contracts
Introduction
The objective of this project is to create a secure and efficient solution for the distribution and verification of certificates. The client, 10 Academy, wants to provide its trainees with a secure way to obtain and verify their certificates. Currently, certificates are simply distributed as PDF files, which cannot be verified for authenticity, nor can 10 Academy undertake smart actions with the trainees and their certificates.

To solve this challenge, 10 Academy has partnered with Algorand to use its blockchain as the foundational element for the creation of Non-Fungible Tokens (NFTs) to represent the successful completion of a weekly challenge for each trainee. This project aims to build an end-to-end Web3 dApp on the Algorand Blockchain that will help 10 Academy generate and distribute NFTs as certificates and allow trainees with NFTs to interact with a smart contract to perform pre-defined actions.

Implementation
This project includes two implementations of Algorand transactions and NFT creation:

Using JS SDK
Using Python SDK
Additionally, a React frontend app is also in development to facilitate the business requirements.

Tech Stack
The following technologies were used to develop this dApp:

React
JS Algo SDK
MyAlgoConnect Wallet API
Pinata IPFS
Purestake API
MySQL (to be deprecated in future work)
The frontend React app is integrated with MyAlgoWallet, which will be used as the login method for trainees.

Folder Structure
The project is organized into the following directories:

api: scripts for FastAPI development
images: screenshots of the frontend app
NFT_js: implementation of creating an asset, transferring an asset, and opt-in using JS SDK
NFT_py: implementation of creating an asset, transferring an asset, and opt-in using Python SDK
notebooks: basic implementation of AlgoSDK in two files, algo_starter and asset notebooks
react: frontend React app
Screenshots
The following are screenshots of the frontend app:

Home Page
Login with MyAlgo
List of Trainees (for trainers)
Detail of a Trainee (for trainers)
Approving or Declining Asset Transfer Request (for trainers)
Installation
Before installing this app, the following must be prepared:

Node.js installed
A config.py file in the api folder with the following information:
Pinata API key and secret
Gmail generated app password
To install and run the app:

Clone this repository: git clone https://github.com/Nathnael12/web3_certificate_generation_verification.git
Go to the project directory: cd web3_certificate_generation_verification
Start the API: cd api then uvicorn app:app --reload
Start the React frontend: cd ../react then npm run start




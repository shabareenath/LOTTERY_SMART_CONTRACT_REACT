# Lottery Smart Contract with React

## Overview

This project showcases a decentralized lottery application that leverages Ethereum smart contracts and a React-based frontend. The smart contract allows participants to enter a lottery by sending Ether, and the contract manager can pick a winner at any time. The React frontend provides an intuitive interface for interacting with the deployed smart contract on the Sepolia testnet.

## Project Structure

- **Smart Contract**: Written in Solidity and deployed on the Ethereum blockchain.
- **Frontend**: Developed using React and Web3.js to provide a seamless user experience.

## Technologies and Libraries

### Smart Contract

- **Solidity**: The smart contract is coded in Solidity, a high-level language for implementing smart contracts on Ethereum. It defines the lottery logic, including entering the lottery, picking winners, and managing participants.
- **Truffle**: Used for Ethereum development, Truffle provides a suite of tools for compiling, deploying, and testing smart contracts. It simplifies the deployment process and provides a testing framework.
- **HDWalletProvider**: This provider is essential for signing transactions with a mnemonic phrase and connecting to the Sepolia testnet. It facilitates the deployment and interaction with the smart contract.

### Frontend

- **React**: A powerful JavaScript library for building user interfaces. React is used to create a responsive and interactive frontend for the lottery application.
- **Web3.js**: A library that allows interaction with the Ethereum blockchain from the frontend. Web3.js is used to communicate with the deployed smart contract and perform blockchain operations.
- **Bootstrap**: A front-end framework for designing the user interface. It helps in creating a modern and visually appealing layout for the application.

### Dependencies

#### Backend

- **@truffle/hdwallet-provider**: This npm package is used to sign transactions and manage the connection to Ethereum networks. It is crucial for deploying and interacting with smart contracts.
- **web3**: An npm package that provides the functionality to interact with Ethereum nodes. It enables communication between the smart contract and the React frontend.
- **solc**: The Solidity compiler, used to compile the smart contract code into bytecode that can be deployed on the Ethereum network.

#### Frontend

- **web3**: As in the backend, this library is used to connect the React frontend with the Ethereum blockchain.
- **bootstrap**: Provides styling and layout features to enhance the visual appeal of the React application.

## Contract Explanation

### Smart Contract Functions

- **`manager`**: Returns the address of the contract's manager. The manager has special privileges, such as picking the winner.
- **`pickWinner`**: Picks a random winner from the participants and transfers the prize to the winner.
- **`getPlayers`**: Retrieves the list of participants currently entered in the lottery.
- **`enter`**: Allows users to enter the lottery by sending Ether to the contract. The sent Ether amount is used as the entry fee.
- **`players`**: Provides the address of a participant at a specific index. Useful for iterating through the list of participants.

### Deployment and Interaction

- **Deployment**: The smart contract is deployed using the Truffle framework and HDWalletProvider, connecting to the Sepolia testnet.
- **Frontend Interaction**: The React application uses Web3.js to interact with the deployed smart contract, allowing users to enter the lottery, view participants, and pick winners.

## Contributing

Contributions to the project are welcome! If you have suggestions for improvements or want to add new features, please open an issue or submit a pull request.





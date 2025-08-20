# Lottery-System-using-a-Smart-Contract-on-Remix-IDE

Decentralized Lottery Smart Contract

This project implements a decentralized Lottery System on the Ethereum blockchain using Solidity and Remix IDE. The goal is to provide a transparent, fair, and secure way for participants to enter a lottery and for a winner to be chosen without relying on a centralized authority.

##🚀 Features

Written in Solidity (v0.8.x)

Uses Ethereum Smart Contracts deployed on Remix IDE or Ganache

Players can participate by sending exactly 1 Ether

Fair winner selection using pseudo-randomness (manual during dev / oracle in production)

Secure manager-only functions (e.g., picking the winner, checking balance)

Automatic reward distribution to the winner

Resets after each round for continuous lotteries

##🛠️ Technologies Used

Solidity (0.8.x) – smart contract language

Remix IDE – for development & testing

Web3.py – Python library for interacting with Ethereum blockchain

EthereumTester / PyEVM – local blockchain backend for testing

Ganache / Infura (optional) – for real testnets


##⚙️ How It Works

Manager Deployment – contract is deployed by a manager (creator).

Player Participation – players join by calling participate() and paying exactly 1 ETH.

Lottery Pool – balance accumulates in the contract.

Winner Selection – manager calls pickWinner() which uses pseudo-randomness to select a winner.

Payout – full contract balance is automatically transferred to the winner.

Reset – players array is cleared, and a new round can start.

##📜 Smart Contract (Core Functions)

participate() → lets players join with 1 ETH

getBalance() → manager-only, checks current pool balance

setManualRandomNumber(uint) → sets manual randomness during testing

pickWinner() → selects and pays out the winner



##📊 Future Improvements

Integrate Chainlink VRF for secure randomness

Add multiple lottery types (daily, weekly, jackpot)

Enable frontend DApp integration with React + Web3.js

##📚 References

Ethereum Docs: https://ethereum.org/developers/

Solidity Docs: https://docs.soliditylang.org/

Web3.py Docs: https://web3py.readthedocs.io/

##👩‍💻 Authors

Varrshinie Aravindan

Team Members: Asmi Takle, Bhavya Verma

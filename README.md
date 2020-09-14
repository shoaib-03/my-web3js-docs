# Web3js with React

# Introduction to web3js

Web3js is a collection of libraries which allow us to interact with a local or remote Etherum node, using a HTTP or IPC connection.

## What is Etherum ?

1. Etherum is the 2nd largest cryptocurrency platform.
2. It is open-source, blockchain based decentrailzed software platfolrm used for its own cryptocurrency ( i.e Ether )
3. It enables Smart Contacts and Distributed Application (DAPPS) to be built and run without any downtime, fraud, control, or interference from third party.
4. It can retrieve user accounts, send transations, interact with samrt contracts, amd more.

## What is Smart Contacts ?

A smart contract is a computer program or a transaction protocol which is intended to automatically execute, control or document legally relevant events and actions according to the terms of a contract or an agreement. (source: Wikipedia)

# web3js API Types

**eth**
> Etherum Blockchain releated methods.

**net**
> Node's network status

**personal**
> Account functions and Sendings

**db** 
> Get/Put for local level DB

**shh**
> P2P messaging using Whisper

# Getting Started

Firstly, we need to initialize a new project using `create-react-app`, and after that we can `install` the web3js package into our project by typing this command 
```
npm install web3
```
One last thing need is a Metamask Extension for Chrome which turn you `Web Browser` to a `Blockchain Browser`.

Now lets jump into coding...

```
import Web3 from 'web3';
```
First of all we have imported  `Web3`

```
const loadBlockchainData = async ()  => {

// Initialize a new Web3 Object
const web3 = new Web3(Web3 givenProvider || 'http://localhost:8545');

// Get Network Type
const network = await web3.eth.net.getNetworkType()

console.log('Network:', network); // Network: main

// Fetch Account
const accounts = await web3.eth.getAccounts();

console.log('Account:', accounts[0]); // Account: key_string
```
}

Now we have created an `async` function to load our account information and inside that we are doing 3 things - 

1. Initializing a new Web3 Object.

2. Getting a network Type using the `getNetworkType()` method of `eth` and `net` API's.

3. Fetching User Account using the `getAccounts()` method of `eth`. The output will a key i.e `String of Characters` of the Account to which you are connected.

Will be continue...






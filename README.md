# Account Abstraction EIP-4337

## Traditional Approcah to manage Crypto assets
1. User recieves 12 word seed phrase
2. This seed phrase generates a private key
3. This private key is the sole authunticator for all the transactions

- Risks for using traditional method
1. Complexity for common users
2. High Stakes if seed phrase is lost
3. Security Risks if lost or compromised
4. Gas fee for each transaction makes the new users with no ETH difficult to start
5. Limited wallet privacy
6. Batching inefficiencies : Performing multiple transactions in a single transaction is not possible in traditional method

## Core shift in Transaction Validation : Account Abstraction
Account abstraction fundamentally redefines how transactions are authorized and validated on a blockchain.
The core idea is to shift from the ECDSA mechanism for signing transactions to a more flexible and programmable system(An arbitary validation logic defined within the smart contract)

- In traditional logic Private key == wallet : Private key is the ultimate authority
- In Acc abs model Progammable logic == wallet : The authority and validation rules are defined by the code within a smart contract account.

## Uses to shift to AA
1. Social login and recovery
2. Multi signature wallets
3. Spending limits
4. Time locks
5. Parental controls

## Gas Abstraction : Solving the *Need Gas* Problem with paymasters
AA enables mechanisms where someone else(*paymaster*) can pay the gas fees on behalf of the user. This is known as gas sponsorship or gas abstraction.
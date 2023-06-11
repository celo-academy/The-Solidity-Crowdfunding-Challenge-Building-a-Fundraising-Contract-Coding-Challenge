## Introduction

Solidity, the primary language for developing smart contracts on blockchain platforms like Celo, is often used to create crowdfunding or fundraising contracts. These contracts enable transparent and immutable transactions, reducing the risk of fraud and misuse of funds. In this challenge, you will be building a simple crowdfunding contract.

## Problem Statement

Design a smart contract that simulates a crowdfunding campaign with the following requirements:

1. The contract owner should be able to start a new campaign with a goal amount and a deadline.
2. Users should be able to contribute to the campaign by sending Celo to the contract until the deadline has passed.
3. If the goal amount is reached or surpassed before the deadline, the contract owner should be able to withdraw the total amount raised.
4. If the deadline has passed without reaching the goal, contributors should be able to withdraw their individual contributions.
5. The contract should not accept contributions after the deadline.

## Hints

- Use `msg.sender` and `msg.value` to handle contributions.
- Use `now` global variable to track the time and enforce the deadline.
- Use a mapping to track each contributor's balance.
- Use `require` statements to enforce the rules of the campaign.
- The `transfer` function can be used to send the raised funds or return the contributors' funds.

## Evaluation Criteria

- **Correctness**: The contract should compile without errors and meet all the requirements.
- **Readability**: The contract should be well-documented, with comments explaining the code.
- **Testability**: You should also provide examples of how to test each function of the contract.

Please note, creating a real-world crowdfunding contract would require additional considerations for security, efficiency, and legal compliance. This challenge is a simplified exercise.

For a comprehensive understanding of Celo smart contracts and Solidity, please refer to the Celo and Solidity tutorials.

## Submission

Please reply with a link to your PR on GitHub, including your crowdfunding contract. Also, include any notes or comments you think are necessary to understand your design and choices. Lastly, provide a brief explanation about how each function of the contract should be tested.

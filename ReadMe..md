# Eligibility Checker

The "EligibilityChecker" smart contract is a piece of code written in Solidity, a programming language specifically designed for creating smart contracts on the Ethereum blockchain. This contract is intended to be deployed on the Ethereum network and provides a simple example of how to check eligibility for voting, buying a car, and taking a pension based on certain criteria.

Here's a more detailed explanation of the various components and functions of the smart contract:

## Smart Contract Details

The smart contract has the following state variables:

* age:  An integer representing the age of the individual. This is used as a basis for checking eligibility for different activities like eligibility for voting, buying a car, and taking a pension.

* hasValidLicense: A boolean value indicating whether the individual has a valid driver's license, which is used for checking eligibility to buy a car.

* hasValidPensionPlan: A boolean value indicating whether the individual has a valid pension plan, used for checking eligibility to take a pension.

### Functions

* checkEligibilityToVote(): This function checks whether the individual is eligible to vote. It uses the require() statement to enforce that the individual's age is at least 18 years. If the condition is not met, the transaction will revert.

* checkEligibilityToBuyCar(): This function verifies whether the individual is eligible to buy a car. It requires the individual to be at least 21 years old and have a valid driver's license. If the conditions are not met, the transaction will revert.

* checkEligibilityForPension(): This function determines if the individual is eligible to take a pension. The eligibility criteria include the individual's age being at least 60 years and having a valid pension plan. If these conditions are not met, the transaction will revert.

### Usage

* Deployment: Deploy the EligibilityChecker smart contract on the Ethereum blockchain using a development tool like Remix or Truffle. You'll need to provide the constructor parameters _age, _hasValidLicense, and _hasValidPensionPlan.

* Calling Functions: Once the contract is deployed, you can interact with it through Ethereum transactions. You can call the checkEligibilityToVote(), checkEligibilityToBuyCar(), and checkEligibilityForPension() functions by sending transactions to the contract address. Depending on the eligibility criteria and input provided, the functions will either succeed or revert.

### Built With

* Solidity: The programming language used to write smart contracts for the Ethereum blockchain.
* Ethereum: The blockchain platform where the smart contract is deployed and executed.

## Help

If you encounter any issues or have questions, please feel free to open an issue in this repository.

## Authors

Tarushi Sandeep Gupta

tarushigupta03@gmail.com

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.

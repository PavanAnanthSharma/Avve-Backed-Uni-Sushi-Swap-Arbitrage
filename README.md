# Aave Flashloan Arbitrage - REVAMPED [OLDER VERSION IS DELETED]

The Aave Flashloan Arbitrage smart contract is a groundbreaking solution for conducting arbitrage between Uniswap and Sushiswap exchanges using Aave's flashloan feature.

## Features:

Flashloans represent a pinnacle of innovation in the Web3.0 and DeFi landscape, offering users the ability to borrow substantial amounts of assets (ERC20) and employ them for various applications, provided the borrowed funds are returned within the same transaction. Aave, Uniswap, Dydx, and other protocols facilitate flashloan functionality.

The FlashLoanArbitrage smart contract harnesses the power of Aave's flashloan capability to execute arbitrage maneuvers between Uniswap and Sushiswap exchanges. The contract is divided into two main components: the first handles arbitrage logic, deposit, and withdrawal functionalities, while the second implements the flashloan logic as outlined in the Aave documentation.

## Built With:

* **Solidity**: The programming language for writing smart contracts, ensuring security and reliability.
* **Brownie**: A Python-based framework for smart contract development, testing, and deployment, offering seamless integration and ease of use.
* **OpenZeppelin**: A library of secure and community-vetted smart contracts, providing robust building blocks for decentralized applications.

## Usage:

### Installation & Setup:

1. **Installing Brownie**: Brownie simplifies smart contract development, testing, and deployments with its Python-based framework. Install Brownie using pipx:
   ```
   pip install --user pipx
   pipx ensurepath
   # restart your terminal
   pipx install eth-brownie
   ```
   Alternatively, install via pip (although pipx is recommended):
   ```
   pip install eth-brownie
   ```

2. **Install ganache-cli**: ganache-cli provides a local Ethereum blockchain for testing purposes. Install it globally using npm:
   ```sh
   npm install -g ganache-cli
   ```

3. **Clone the repository**: Clone the Aave Flashloan Arbitrage repository to your local machine:
   ```sh
   git clone https://github.com/PavanAnanthSharma/Avve-Backed-Uni-Sushi-Swap-Arbitrage/tree/main
   cd Avve-Backed-Uni-Sushi-Swap-Arbitrage
   ```

4. **Set environment variables**: Configure your environment variables by adding your PRIVATE_KEY (obtained from your Ethereum wallet like Metamask) and the Infura project ID (sign up for an Infura account) to the .env file:
   ```
   PRIVATE_KEY=<YOUR_PRIVATE_KEY>
   WEB3_INFURA_PROJECT_ID=<YOUR_INFURA_PROJECT_ID>
   ```

### How to Run:

To initiate arbitrage on the mainnet fork (for testing purposes only, you can also use the Kovan testnet), execute the following command:
   ```sh
   brownie run scripts/flashloan_arbitrage.py --network=mainnet-fork
   ```

This concise guide provides all the necessary steps to install, set up, and run the Aave Flashloan Arbitrage smart contract, empowering users to harness the potential of flashloans for lucrative arbitrage opportunities in the decentralized finance ecosystem.

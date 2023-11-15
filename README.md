# DSN Token 🏦

This repository contains the contract code for the DSN Token

The $DSN token—the governance token of the Descent Protocol, allows those who hold it to vote on changes to the Descent Protocol. 
Note that anyone, not only $DSN holders, can submit proposals for an $DSN vote.

## Design Considerations

The $DSN token has 3 methods of use within the Descent Protocol 

- As a utility token
    - As xNGN stability fees earned on Vaults accrue within the Descent Protocol, 
    $DSN holders can use $DSN to vote to enable the the auction module to sell xNGN surplus for $DSN.  Once the auction is complete the $DSN protocol burns the $DSN.

- As a governance token
    - $DSN is used by $DSN holders to vote for the risk management and business logic of the Descent Protocol. Tokens are a simple representation of voting power.

- As a recapitalization resource
    - $DSN can autonomously be minted by the auction module and sold for xNGN, which is used to recap the Descent Protocol in times of insolvency.


## Usage

### Prerequisites

-   [git](https://git-scm.com/downloads)
-   [nodeJS](https://nodejs.org/en/download/)
-   [brew](https://brew.sh/)
-   [foundry](https://getfoundry.sh) - You can run `sh ./setup.sh` to install Foundry and its dependencies.
-   [Hardhat](https://hardhat.org)

### Setup

-   Clone the repository

    ```bash
    git clone https://github.com/Descent-Collective/DSN-token.git
    cd DSN-token
    ```

-   Install packages

    ```
    yarn
    ```

 -   Build contracts

    ```
    yarn build
    ```


### Deploying

Create a .env in the root with:

```
PRIVATE_KEY=PRIVATE_KEY
ALCHEMY_API_KEY=
```

Then run:
```
yarn run deploy:ethereum_goerli
```

## Run unit tests

```shell
yarn run test
```

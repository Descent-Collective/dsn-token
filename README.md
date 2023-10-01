# OSN Token 🏦

This repository contains the contract code for the OSN Token

The $OSN token—the governance token of the Onboard Protocol, allows those who hold it to vote on changes to the Onboard Protocol. 
Note that anyone, not only $OSN holders, can submit proposals for an $OSN vote.

## Design Considerations

The $OSN token has 3 methods of use within the OSN Protocol 

- As a utility token
    - As xNGN stability fees earned on Vaults accrue within the Onboard Protocol, 
    $OSN holders can use $OSN to vote to enable the the auction module to sell xNGN surplus for $OSN.  Once the auction is complete the $OSN protocol burns the $OSN.

- As a governance token
    - $OSN is used by $OSN holders to vote for the risk management and business logic of the Onboard Protocol. Tokens are a simple representation of voting power.

- As a recapitalization resource
    - $OSN can autonomously be minted by the auction module and sold for xNGN, which is used to recap the Onboard Protocol in times of insolvency.


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
    git clone https://github.com/Descent-Collective/osn-token.git
    cd osn-token
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

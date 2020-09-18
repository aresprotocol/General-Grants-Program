
# Project Name

Ares Protocol

## Project Description

Ares Protocol is a decentralized oracle project based on Substrate. The goal is to provide real data off-chain for smart contracts, parachains or other projects in the Substrate ecosystem.

The Ares Protocol network is composed of data users, providers and verifiers. The user requests data, and the data provider is responsible for providing real-world data sources off the chain. Oracle aggregates data from multiple data sources, generates the final data after a certain weighting algorithm, and submits it to the chain for other smart contracts on the chain or DApp use. In the process of aggregating data, it is necessary to use the true random number encapsulated in BABE to select a validator responsible for generating the block.

#### Random number package

In the Substrate BABE consensus algorithm engine, a true random number has been generated. Ares Protocol will package this random number generator and provide it to other users on the chain. In the process of Ares generating blocks, it is necessary to randomly select one of 99 validators to generate the block, and this random number will be used in this selection process.
#### Data provider

Each data provider will choose to provide a certain type of data. The provider can join the data provider role autonomously and must pledge a certain amount of ARES Token as the data source to provide a guarantee for real offline data. At any time, the data provider can withdraw from the data provider role, and then get back the ARES mortgaged.

Each data provider will have two indicators that affect the weight of the data it provides and the amount of rewards it receives:

1. The amount of mortgaged Token

The Ares network calculates its weight based on the number of pledged tokens for a certain data type. The greater the number of mortgage tokens, the greater the confidence in the correctness of the data provided by oneself.

2. Credit index

The credit index is a measure of the authenticity of the data provided by the data provider.

#### reward

After each data provision is completed, the data requester needs to pay a certain fee as a reward to the data provider and verifier.

#### Oracle script

For the data demander (User), every time there is a data demand, a data request will be sent to the Oracle Script. After the request is sent, all data providers of the same type will receive the request and obtain data from their own data source.

#### data verification

After receiving enough data replies, verify the data by means of three-layer node verification and calculate the final data submitted to the chain.

The data verifier role is responsible for packing the process information of each data request into a block to record all information verification records.

#### Return data to the data requester

After the data is verified, the block is generated and written to the chain. The data is returned to the original data requester.

## Ecosystem Fit
Are there any other projects similar to yours? If so, how is your project different?


## Team members
* Andy Ray
* Eric Li
* Scott Dai
* Fred Lei
* Kevin Zhang

## Team Website
* https://aresprotocol.com

## Legal Structure
Please provide the name and registered address of the legal entity executing the project. These details can also be shared privately via the Google Form used for your application.

## Team's experience
Please describe the team's relevant experience.  If the project involves development work, then we'd appreciated if you can single out a few interesting code commits made by team members on their past projects.  We'll glance at whole repositories too, but not if they contain many vendored dependencies, which often makes commits easier.
* We have 15+ years software Development experience, include Embedded Devices, Distributed System, Mobile System.
* Be engaged in blockchain development since 2016, familiar with Ethereum and Hyperledger Fabric development work

## Team Code Repos
* https://github.com/aresprotocol/aresprotocol

## Team LinkedIn Profiles
* TBD

## Target Programming Language
Rust, Golang

## Development Roadmap

#### Milestone 1 — Design the Architecture

Design the overall system architecture of Ares and the interface definition between the major modules.
The developing cost is about 5k dollars
#### Milestone 2 — Implement

The following large modules can be developed in parallel

* Develop smart contracts on Substrate and provide data usage interfaces for various other users (smart contracts, DApp, etc.)
* Development of off-chain data acquisition modules, including data provider registration, acquisition of real-world data sources, etc.
* Data verification module, including three-layer node verification model and block generation and chaining

The developing cost is about 15k dollars


#### Milestone 3 — Testing

Work with third-party partners to test and verify the entire Ares Protocol.

The developing cost is about 10k dollars

## Additional Information


Any additional information that you think is relevant to this application that hasn't already been included.

Possible additional information to include:
* What work has been done so far?
* Are there are any teams who have already contributed (financially) to the project?
* Have you applied for other grants so far?

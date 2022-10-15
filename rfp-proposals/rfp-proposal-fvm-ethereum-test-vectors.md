# RFP Proposal: `Tool for applying test vectors from Ethereum on FEVM`

**Name of Project:** Tool for applying test vectors from Ethereum on FEVM

**Link to RFP:**  https://github.com/filecoin-project/devgrants/pull/1063

**RFP Category:** `category:devtools-libraries`

**Proposer:** [@coder-lb](https://github.com/storswiftlabs)

**Do you agree to open source all work you do on behalf of this RFP and dual-license under MIT and APACHE2 licenses?:** 
Yes

# Project Description

FVM 2.1 which introduces support for Ethereum smart contracts in the Filecoin network (FEVM) will be the biggest network upgrade since mainnet launch. At the same time, it immensely widens the area of possible problems. That’s why it must be tested thoroughly.
One of possibilities to test FEVM is to run already existing and proven smart contracts from Ethereum and compare the state it produces on Ethereum vs Filecoin.

We are seeking proposals from teams that can build such a testing tool. This tool is expected to be in the form of a CLI.
It should be able to:

1. Fetch and store on the order of hundreds of contracts from Ethereum mainnet. These should be widely used contracts covering various use-cases. 
2. Deploy these contracts to a Filecoin testnet (Butterflynet).
3. Fetch thousands of transactions sent to these contracts on Ethereum in the past. 
4. Replay these transactions to contracts deployed on Filecoin. 
5. Compare the Ethereum state before and after these transactions with the results on Filecoin. We expect the team to research the ideas of how to do state comparison reliably.

We want to run this tool a few times if needed and fix encountered errors every time.
This tool can be written in either Go or Rust.

# Draft proposal graph

![image](https://user-images.githubusercontent.com/67536047/195347846-3ea34be4-f70c-4381-8c77-a11aa99c37c4.png)

![image](https://user-images.githubusercontent.com/67536047/195347977-d1b0df99-0adb-41c3-a4f7-11893f176196.png)

![image](https://user-images.githubusercontent.com/67536047/195348190-17f08fc1-d5df-43a7-9e78-2212fe03b816.png)


## Deliverables

* Source code of the tool
* Guides on how to use it
* Fetched smart contracts and transactions 


## Development Roadmap



## Milestones & Funding

<table>
  <tr>
   <td><strong>Milestone No.</strong>
   </td>
   <td><strong>Milestone Description</strong>
   </td>
   <td><strong>Funding</strong>
   </td>
   <td><strong>Estimated Timeframe</strong>
   </td>
  </tr>
  <tr>
   <td>1
   </td>
   <td>Design the test tool architecture and finalize the specification
   </td>
   <td>1 FTE: 10000 \$
   </td>
   <td>3 days
   </td>
  </tr>
  <tr>
   <td>2
   </td>
   <td>Implementation of a function which fetches hundreds of contracts and transactions from Ethereum, stores them 
   </td>
   <td>2 FTE: 9800 \$
   </td>
   <td>5 days
   </td>
  </tr>
  <tr>
   <td>3
   </td>
   <td>Implementation of a function which deploys contracts to Filecoin testnet and replays transactions on Filecoin testnet
   </td>
   <td>2 FTE: 9600 \$
   </td>
   <td>5 days
   </td>
  </tr>
  <tr>
   <td>4
   </td>
   <td>Implementation of a function which compares the Ethereum state before and after these transactions with the results on Filecoin
   </td>
   <td>2 FTE: 14800 \$
   </td>
   <td>8 days
   </td>
  </tr>
  <tr>
   <td>5
   </td>
   <td>Finish the test and work out the guides about how to use
   </td>
   <td>1 FTE: 3800 \$
   </td>
   <td>4 days
   </td>
  </tr>
</table>

## Total Funding Requested
Total: 48000 \$

## Maintenance and Upgrade Plans

Our team will maintain the tool consistently and upgrade it over time to make it a really cool product.

# Team

## Contact Info

Email: lengbo@storswift.com

## Team Members

- Team Member 1: macro-ss
- Team Member 2: marco-swift 
- Team Member 3: alexzhenyu

## Team Member Github Profiles

- Team Member 1 Github Profile: https://github.com/macro-ss
- Team Member 2 Github Profile: https://github.com/marco-storswift
- Team Member 3 Github Profile: https://github.com/alexzhenyu

## Relevant Experience

- experience in NLP and machine learning, familar with all kinds of public datasets.
- experience in design big data warehouse, familar with big data modeling and deep mining.
- experience in EVM, substrate framework, Filecoin, FVM development
- experience of python/javascript/golang/rust/Java

## Team code repositories

https://github.com/storswiftlabs

# Additional Information
Our team start to research and develop for Web3 two years ago. We have implemented the optmized version of PoREP/PoST code, worker task secheduling code, devops management system, and so on. From the very beginning, we have been focused on Filecoin security solutions. We research offline signature, cold wallet and multisig solutions. We also develop a framework to ensure the security of devops for Filecoin clusters.

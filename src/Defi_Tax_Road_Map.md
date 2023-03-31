# RoadMap 
- DeFiTax 
- Decentralized Tax Calculator(USA)

---
1. Purpose
Building a decentralized tax calculating platform on the Polkadot framework which powers the individual by giving the entire taxable calculation on their defi(transactions, staking) activities on crypto assets. Our platform will provide the users with the one-stop solution for their tax estimate of all the transactions and staking activities. All the complex tax calculations are handled by our tax engine. 

2. Outline of Work


`Tax Engine implementation:` Working on the designing the tax engine for laying out the core logic, handling the tax calculation
- `Indexing solution implementation for Subscan:` Using the SubQuery SDK and platform for building various indexing solution for various transactions and hosting respectively  
- `Blockchain: `
Implementation of the logic and building various pallets to create and handle extrinsics 
- `UI implementation:` Creating the frontend app for the users to interact and submit their request for the tax estimate

---
3. Expected Execution Timeline 

- Week 1 & 2  -  Laying out the plan and designing the end-to-end architecture. 

- Week 3 & 4  -  Start building the indexer and working on the tax engine

- Week 5 & 6 -  Creating blockchain and writing the core logic for the extrinsics      and continue to work on the tax engine

- Week 7 & 8 -  UI integration with indexer and smart contract 

- Week 9 & 10-  Integrating the app with tax engine and working on testnet 

- Week 11    Implementation in mainnet

- Week 12  -  Bug Ironing + Documentation (Gitbook) 

---


4.  Technologies and Tools


| Frontend | Backend | 
|---------|---------|
| ReactJS, Javascript, Bootstrap, Web3js, Tailwind CSS    | RUST, Substrate , Python(if needed)  |

| Indexing and API |  |
|---------|---------|
| SubQuery, GRAPHQL, REST Technologies     |    |

---

6. Future

- Adding more utility for the native token
- Storing the snapshot of the report for taxable income generated as NFT 
- Expanding to different countries 







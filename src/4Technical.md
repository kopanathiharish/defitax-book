
# Technical
```
diagram
```


As per the technical architecture above, we have our user connecting to the wallet and then they can choose for the chain, it can be a relaychain like polkadot or kusama or maybe any other chains built on polkadot or kusama.

For the current iteration we are only focussing on polkadot and kusama which we will extend for all the other chains as well.

Once the wallet is connected and the chain is chosen, then they can start the tax calculation by just pressing a button which will initiate the process. As a part of the first step they need to specify all the wallets the user has.

Which they can do either manually or by selecting among the transactions, which our app will help to do so.

After doing that they will get the taxable amount which they can either use our platform to pay(future goal of integrating with the tax paying systems based on their decentralizations) or they can export and use it for paying the tax by themselves.

So coming to the technical how it works is we have our react app connecting to polkadot.js extension or any supported wallet. After connecting, the user starts processing, we submit an extrinsic from our pallet which will call the SubQuery GraphQL API which is built and hosted on the Subquery platform.

The SubQuery API will index the transactions for the DOT address from the wallet and give those transaction back to our front-end.

We have onFinality api behind the subquery which runs the nodes and helps us indexing the transaction based on the wallet address provided. After the successful response from subquery graphql api.

We fetch the information from our pallet and feed that to the tax engine.

Tax engine is the core component of our app which then does all the hard handling and provides us with the taxable amount with multiple options to deal further as explained above.

# Substrate/Polkadot Integration

Polkadot ecosystem and the newly-updated Substrate 2.0 are essential to what the Network is trying to achieve.

The network will be connected to the Polkadot ecosystem acting as a para chain, sharing the Polkadot underlying consensus, and protected by the network performance of Polkadot and Substrate.

Polkadot/Kusama is an important foundation, on which the Network and its components are built.

The pallets that come with the Substrate 2.0 upgrade can offer Network the tools and maps to navigate through our vision, which is to build an advanced decentralized oracle that offers on/off-chain data with built-in interoperability.

The off-chain worker is a substrate subsystem that can process off-chain data in an asynchronous way.

It is a new feature in Substrate Framework that allows integrating data onto the blockchain. It can make off-chain data integration secure and more efficient, which is ideal for real-world data inputs via oracles.

The off-chain worker subsystem allows execution of long-running and possibly non-deterministic tasks (e.g. web requests, encryption/decryption and signing of data, random number generation, CPU-intensive computations, enumeration/aggregation of on-chain data, etc.) leveraging on-chain data and access.

Thus, we have the Data Warehouse in the system which will deal with Date Feeds and Data Requests sent by the user in a local data store or even a decentralized data storage such as IPFS.
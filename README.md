                                                    # Auto Replenishment of Inventory using Blockchain
 
### Introduction

Walmart’s global presence, with its vast number of retail stores plus its robust and rapidly growing e-commerce business, make it one of the most challenging retail companies on the planet for inventory-related use cases.

Blockchain has been technological basis for many digital currencies, but it is also emerging as an alternative to widely used technology for many other domains. We tried exploring more about the topic of Blockchain, but, being such a generic technology, we needed a specific area of application. After pondering both the benefits it could bring and the needs it could satisfy, we chose to develop a proof-of-concept (PoC) that could apply blockchain technology to a supply chain.

### HyperLedger Fabric

Hyperledger Fabric is a blockchain platform for developing decentralized applications (dapps). You can use smart contracts to implement an auto-replenish inventory system on Hyperledger Fabric.

A smart contract in this system would hold the inventory levels and automatically execute the reordering process when the inventory reaches a certain threshold. The smart contract would trigger the ordering process, and the transaction would be recorded on the blockchain, ensuring transparency and immutability.

For example, the smart contract could be programmed to automatically place an order for more inventory with a supplier when the current inventory drops below a certain level. The supplier would then fulfill the order, and the updated inventory levels would be recorded in the blockchain, making the entire process secure and tamper-proof.

Overall, using smart contracts on Hyperledger Fabric provides a secure, transparent, and automated solution for managing inventory replenishment.

### Smart Contracts
Further, since all transactions are executed sequentially by all nodes, performance and scale is limited. The fact that the smart contract code executes on every node in the system demands that complex measures be taken to protect the overall system from potentially malicious contracts in order to ensure resiliency of the overall system.


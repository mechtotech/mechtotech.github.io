# Iventory Management System using Blockchain

Walmart’s global presence, with its vast number of retail stores plus its robust and rapidly growing e-commerce business, make it one of the most challenging retail companies on the planet for inventory-related use cases.

Blockchain has been technological basis for many digital currencies, but it is also emerging as an alternative to widely used technology for many other domains. We tried exploring more about the topic of Blockchain, but, being such a generic technology, we needed a specific area of application. After pondering both the benefits it could bring and the needs it could satisfy, we chose to develop a proof-of-concept (PoC) that could apply blockchain technology to a supply chain.

### Smart Contracts
A smart contract, or what Fabric calls “chaincode”, functions as a trusted distributed application that gains its security/trust from the blockchain and the underlying consensus among the peers. It is the business logic of a blockchain application.

There are three key points that apply to smart contracts, especially when applied to a platform:

many smart contracts run concurrently in the network,
they may be deployed dynamically (in many cases by anyone), and
application code should be treated as untrusted, potentially even malicious.
Most existing smart-contract capable blockchain platforms follow an order-execute architecture in which the consensus protocol:

validates and orders transactions then propagates them to all peer nodes,
each peer then executes the transactions sequentially.
The order-execute architecture can be found in virtually all existing blockchain systems, ranging from public/permissionless platforms such as Ethereum (with PoW-based consensus) to permissioned platforms such as Tendermint, Chain, and Quorum.

Smart contracts executing in a blockchain that operates with the order-execute architecture must be deterministic; otherwise, consensus might never be reached. To address the non-determinism issue, many platforms require that the smart contracts be written in a non-standard, or domain-specific language (such as Solidity) so that non-deterministic operations can be eliminated. This hinders wide-spread adoption because it requires developers writing smart contracts to learn a new language and may lead to programming errors.

Further, since all transactions are executed sequentially by all nodes, performance and scale is limited. The fact that the smart contract code executes on every node in the system demands that complex measures be taken to protect the overall system from potentially malicious contracts in order to ensure resiliency of the overall system.


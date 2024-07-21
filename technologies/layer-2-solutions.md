# Layer 2 Solutions

By utilizing smart contracts on L2 networks such as Optimism and Linea, we provide on-chain storage for resolving the owner addresses of subdomains associated with ENS domains. This approach significantly reduces costs compared to the Ethereum mainnet.

### **Overview of Layer 2 Solutions**

Layer 2 solutions are secondary frameworks or protocols built on top of existing blockchain networks. They aim to enhance the performance of the primary blockchain (Layer 1) by offloading transaction processing, thereby increasing throughput and reducing fees.

### **Key Functions and Benefits**

1. **Efficient On-Chain Storage**:
   * Instead of storing ENS domain data on the Ethereum L1, we use L2 smart contracts to manage and resolve domain owner addresses.
   * This shift to L2 networks like Optimism and Linea allows for faster and cheaper transactions.
2. **Cost-Effective and Scalable**:
   * L2 networks are more cost-effective than the Ethereum mainnet, significantly reducing gas fees for users.
   * Enhanced scalability ensures that our platform can handle a higher volume of transactions without compromising performance.

### **Technical Implementation**

1. **Minting NFTs on L2**:
   * Users mint an NFT for their subdomains on an L2 network. This NFT represents ownership of the subdomain.
   * The smart contract on the L2 network securely stores the ownership details of each subdomain.
2. **Domain Resolution Process**:
   * When an ENS resolution request is made, the resolver contract queries our CCIP gateway.
   * The serverless function reads the required domain details from the L2 smart contract associated with the NFT.
   * The gateway then sends the retrieved data back to the ENS resolver, which updates the domain records.
3. **Trusted Gateway and Future Developments**:
   * Currently, our flow depends on a trusted gateway to facilitate the resolution process.
   * Ongoing developments aim to transition to trustless solutions, leveraging advanced cryptographic techniques and decentralized protocols to eliminate the need for a trusted intermediary.

**Benefits and Use Cases**

1. **Lower Costs**:
   * Transactions on L2 networks incur significantly lower fees compared to the Ethereum mainnet, making it affordable for users to mint and manage their subdomains.
2. **Enhanced User Experience**:
   * Users can easily mint an NFT for their subdomains and own an ENS-based subdomain, with the added benefit of support from platforms like OpenSea and MetaMask.
   * This integration simplifies the management and utilization of subdomains in the Web3 ecosystem.
3. **Scalability for Business Needs**:
   * The scalability of L2 solutions makes them ideal for businesses that need to manage a large number of subdomains efficiently.
   * The reduced costs and increased performance support the growing demand for decentralized domain management.

By leveraging Layer 2 solutions, 3ID enhances the efficiency, affordability, and scalability of managing ENS-based subdomains. This approach ensures that our platform remains at the forefront of decentralized domain management, providing a robust and user-friendly solution for the Web3 community.

---
description: Chainlink Cross-Chain Interoperability Protocol
---

# CCIP Read (EIP-3368)

The Chainlink Cross-Chain Interoperability Protocol (CCIP) Read, also known as EIP-3368, is a pivotal technology used in the 3ID platform. This protocol facilitates the efficient retrieval of domain data and records from off-chain sources, enhancing the functionality and user experience of our services.

### **Overview of CCIP Read**

CCIP Read is an advanced protocol designed to enable secure and efficient communication between different blockchain networks and off-chain data sources. By leveraging CCIP Read, 3ID can ensure that domain information is accurately resolved and propagated across multiple platforms.

### **Key Functions and Benefits**

1. **Facilitating Data Retrieval**:
   * CCIP Read allows the 3ID platform to retrieve domain data and records from off-chain gateways such as Cloudflare workers and Vercel serverless functions.
   * This capability ensures that the resolution of ENS subdomains is efficient and accurate, even when data is stored off-chain.
2. **Enabling Cross-Chain Name Propagation**:
   * CCIP Read supports the registration of on-chain names on one blockchain and their propagation across other blockchains.
   * This functionality ensures that users can maintain consistent and interoperable domain identities across different blockchain networks.
3. **Enhancing Security and Reliability**:
   * By using CCIP Read, 3ID can securely access and verify off-chain data, maintaining the integrity and trustworthiness of the domain records.
   * The protocol’s robust security measures protect against data tampering and unauthorized access.

### **Technical Implementation**

* When a domain resolution request is made, the ENS resolver contract uses CCIP Read to query the relevant off-chain gateway (e.g., Cloudflare worker).
* The off-chain gateway processes the request, retrieves the necessary data from its storage (e.g., Cloudflare D1 database), and sends the data back to the ENS resolver.
* You can check out more detailed information about CCIP read at [ENS Documentation](https://docs.ens.domains/resolvers/ccip-read) and [Ethereum documentation](https://eips.ethereum.org/EIPS/eip-3668).

By leveraging CCIP Read (EIP-3368), 3ID ensures that domain resolution is efficient, secure, and interoperable across multiple blockchain networks. This technology underpins the platform's ability to offer advanced domain management solutions, enhancing the overall user experience and reliability of our services.

***

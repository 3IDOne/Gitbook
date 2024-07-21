# On-chain Subdomain

In addition to our off-chain subdomain services, 3ID offers an innovative solution for registering low-cost ENS-based subdomains on Layer 2 (L2) networks. This service combines the security and reliability of on-chain data with the affordability and scalability of L2 solutions.

### **Registration Process**

1. **User Registration**:
   * Users can register an L2 subdomain by signing a transaction with a small fee. This fee is significantly lower than the high gas costs associated with the Ethereum mainnet and traditional ENS platform registration.
   * Users can choose from various extension options and select an L2 chain, such as Optimism or Linea.
2. **NFT Representation**:
   * Upon successful registration, users receive an NFT on the selected L2 chain. This NFT represents the ownership of the subdomain.
   * The NFT is transferable, allowing the ownership of the subdomain to be changed by transferring the NFT to another user.
3. **Data Storage**:
   * Ownership data is stored on a smart contract deployed on the L2 network. This ensures that the ownership information is secure, verifiable, and easily transferable.
4. **Domain Resolution**:
   * When ENS needs to resolve the domain's information, it sends a request to the resolver contract.
   * The resolver contract calls a serverless function that interacts with the NFT smart contract to retrieve the owner address associated with the domain name.
   * ENS off-chain resolver contracts, utilizing Cross-Chain Interoperability Protocol (CCIP) technology, facilitate this process by ensuring the smooth retrieval of on-chain data.

### **Technical Flow**

1. **Signing a Transaction**:
   * Users sign a transaction on their chosen L2 network to request the registration of a subdomain. This transaction includes a small fee, making the process affordable compared to Ethereum mainnet fees.
2. **NFT Issuance**:
   * Upon transaction confirmation, an NFT representing the subdomain ownership is minted and assigned to the user.
   * This NFT can be transferred to others, enabling flexible ownership management.
3. **Smart Contract Data Storage**:
   * The NFT smart contract on the L2 network stores the ownership information. This contract ensures that the owner address associated with each subdomain is easily retrievable.
4. **ENS Resolution Request**:
   * When ENS needs to resolve the subdomain, it sends a request to the ENS off-chain resolver contract.
   * The resolver contract calls a serverless function to interact with the L2 NFT smart contract.
5. **Serverless Function Execution**:
   * The serverless function queries the NFT smart contract for the owner address linked to the subdomain.
   * This function retrieves the ownership data from the smart contract and responds to the resolver contract.
6. **ENS Record Display**:
   * The resolver contract sends the retrieved owner address to ENS.
   * ENS caches and displays the records, providing accurate and up-to-date information about the subdomain's ownership.
7. **CCIP Technology**:
   * CCIP technology ensures that data integrity and security are maintained during the resolution process.
   * This technology enables seamless integration of on-chain and off-chain data, providing a robust and scalable solution for subdomain management.

By leveraging L2 networks and NFT-based ownership, 3ID offers a cost-effective and efficient solution for managing ENS-based subdomains. This approach not only reduces registration costs but also enhances the flexibility and security of domain ownership.

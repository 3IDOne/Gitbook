# Off-chain Subdomain

### Off-Chain Subdomains

At 3ID, we offer a novel solution to register free ENS-based subdomains with various extension options. This service is designed to be user-friendly and cost-effective, eliminating the need for on-chain transactions and associated fees.

### **Registration Process**

1. **User Registration**:
   * Users can register a free ENS-based subdomain by simply signing a message. This process does not require an on-chain transaction, thereby avoiding gas fees.
   * The user selects a desired subdomain and an extension from the available options.
2. **Data Storage**:
   * Once the user signs the message, a Cloudflare worker function is triggered.
   * The worker stores the user's subdomain data in a Cloudflare D1 database, an efficient and scalable off-chain storage solution.
3. **Domain Resolution**:
   * When a request is made to resolve the subdomain's information, ENS interacts with its resolver to fetch the necessary records.
   * The resolver queries the Cloudflare worker, which responds with the data stored in the Cloudflare D1 database.
   * The ENS off-chain resolver contracts, leveraging Cross-Chain Interoperability Protocol (CCIP) technology, facilitate this process by ensuring the smooth retrieval and validation of off-chain data.

### **Technical Flow**

1. **Signing a Message**:
   * The user signs a message to request the registration of a subdomain. This message is cryptographically secure and verifies the user's intent without requiring an on-chain transaction.
2. **Cloudflare Worker Execution**:
   * The signed message triggers a Cloudflare worker function.
   * The worker processes the request, validates the subdomain, and stores the relevant data (such as subdomain, owner information, and other metadata) in the Cloudflare D1 database.
3. **Data Storage in Cloudflare D1 Database**:
   * The Cloudflare D1 database serves as the off-chain storage for subdomain records. This database is optimized for high availability and rapid data retrieval.
4. **ENS Resolution Request**:
   * When ENS needs to resolve the subdomain, it sends a request to the associated resolver.
   * The resolver, using off-chain resolver contracts and CCIP technology, queries the Cloudflare worker for the stored data.
5. **Cloudflare Worker Response**:
   * The Cloudflare worker retrieves the requested data from the D1 database and responds to the resolver.
   * The resolver then returns the data to ENS, which caches and displays the records.
6. **CCIP Technology**:
   * CCIP technology underpins the off-chain resolution process, ensuring that data integrity and security are maintained while facilitating cross-chain interactions.
   * This technology enables the seamless integration of off-chain data with on-chain processes, providing a robust and scalable solution for managing subdomain records.

By leveraging off-chain storage and advanced technologies like CCIP, 3ID offers a streamlined and cost-effective solution for managing ENS-based subdomains. This approach not only reduces costs but also enhances the user experience by simplifying the registration and resolution processes.

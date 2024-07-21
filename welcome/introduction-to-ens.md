---
description: ENS, the underlying technology of 3ID platform
---

# Introduction to ENS

### Overview of Ethereum Name Service (ENS)

The Ethereum Name Service (ENS) is a distributed, open, and extensible naming system based on the Ethereum blockchain. ENS's primary goal is to map human-readable names, such as `alice.eth`, to machine-readable identifiers, including Ethereum addresses, other cryptocurrency addresses, content hashes, and metadata. This system simplifies the user experience in interacting with blockchain-based assets and smart contracts.

#### Components of ENS

1. **Registry**:
   * The ENS registry is a smart contract that maintains a list of all domains and subdomains, as well as stores essential information about each domain, including the owner, resolver, and the time-to-live (TTL) for all records under the domain.
   * The registry is intentionally simple and straightforward, ensuring robustness and security.
2. **Registrars**:
   * Registrars are smart contracts responsible for managing the allocation of subdomains. A registrar can be thought of as a domain controller that governs how subdomains are created and assigned.
   * For example, the `.eth` registrar manages the allocation of second-level domains under `.eth`.
3. **Resolvers**:
   * Resolvers are smart contracts that translate ENS names into the respective addresses or other resources. Each record type (e.g., address resolution, IPFS content hash) can be resolved via these contracts.
   * Users can choose different resolvers for their domains, depending on their needs, with the flexibility to update resolvers as necessary.

#### Sections of ENS

1. **Name Registration**:
   * This section involves registering a new ENS name, either through direct purchase or participating in an auction (for premium or highly-demanded names).
   * Users interact with the registrar responsible for the domain they want to register.
2. **Name Management**:
   * Once a name is registered, the owner can manage it via the ENS management interface. This includes setting and updating the resolver, transferring ownership, and managing subdomains.
   * Name owners can set different records such as Ethereum addresses, cryptocurrency addresses, IPFS content hashes, and text records.
3. **Resolution**:
   * The resolution process involves querying the ENS registry to find the appropriate resolver for a name and then using the resolver to retrieve the associated address or resource.
   * This ensures that services and applications can seamlessly translate ENS names into the required data.

#### Functionality Flow

1. **Registration**:
   * A user initiates the registration process by sending a transaction to the ENS registrar smart contract.
   * Depending on the registration type (e.g., auction for `.eth` names), the user might place a bid or pay a fixed fee.
   * Upon successful registration, the user becomes the owner of the name and can configure its settings.
2. **Setting Up a Resolver**:
   * The domain owner selects a resolver contract to handle their ENS records.
   * The resolver's address is set in the ENS registry for the specific domain.
3. **Creating Records**:
   * The domain owner creates and updates various records (e.g., addresses, content hashes) via the resolver contract.
   * These records can be queried by anyone to obtain the relevant information associated with the ENS name.
4. **Resolution Process**:
   * A user or application queries the ENS registry to find the resolver for a given ENS name.
   * The resolver is then queried to retrieve the specific records (e.g., an Ethereum address) associated with the name.
   * The retrieved information is used to perform the desired action, such as sending a transaction to the resolved Ethereum address.

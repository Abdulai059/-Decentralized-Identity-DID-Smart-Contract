# Identity Management Smart Contract

Overview
The Identity Management Smart Contract is a decentralized identity management system built on Ethereum. It allows users to register, verify, revoke, and manage their identities securely while maintaining a robust access control mechanism for authorized verifiers and administrators.

### **Contract Details**
- **Contract Address**: `0x6224A57603d2D60eC11a7a00A2065f0C16Cc8D42`
- **Network**: Arbitrum Sepolia 


## Features

1. **Identity Management**  
   - Register a new identity with details such as name, email, and a verification document reference.
   - Verify or revoke an identity status.

2. **Access Control**  
   - Only authorized verifiers can verify or revoke identities.
   - Only the contract manager can manage verifiers.

3. **Transparency**  
   - Emits events for registration, verification, revocation, and verifier updates.
   - Publicly retrieves identity information for registered users.



## How to Use

### 1. Register an Identity  
Use the `registerIdentity` function to register your identity


### 2. Verify an Identity  
Authorized verifiers can mark an identity as verified

### 3. Revoke an Identity  
Authorized verifiers can revoke an identity’s status

### 4. Retrieve Identity Information  
Fetch details of a registered identity

### 5. Add or Remove Verifiers  
Only the contract manager can add or remove verifiers


## Events

- **IdentityRegistered**: Emitted when a new identity is registered.
- **IdentityVerified**: Emitted when an identity is verified.
- **IdentityRevoked**: Emitted when an identity is revoked.
- **VerifierAdded**: Emitted when a new verifier is added.
- **VerifierRemoved**: Emitted when a verifier is removed.


## Access Control

- **Manager**: The deployer of the contract who can manage verifiers.
- **Verifiers**: Authorized addresses allowed to verify or revoke identities.
- **Identity Owner**: Users who own their registered identities.


## Development and Testing

1. Deploy the contract using Remix or your preferred tool.
2. Use the provided contract address to interact with the deployed contract.
3. Test functionality using accounts with different roles (e.g., manager, verifier, user).


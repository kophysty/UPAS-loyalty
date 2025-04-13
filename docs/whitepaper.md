# UPAS: Universal Protocol for Achievements and Reputation on the Internet Computer

## 1. Executive Summary

UPAS (User Public Achievement Standard) is an open protocol for digital loyalty and reputation, built on the Internet Computer (ICP). It enables businesses to issue verifiable credentials and reward users for real-world behavior while maintaining user privacy and regulatory compliance. With the first milestone completed and pilot programs based on UPAS underway, the protocol is becoming a foundational standard for Web3-native loyalty solutions.

## 2. Problem & Market Opportunity

The loyalty program industry is massive — projected to exceed $200B by 2027 — yet outdated, siloed, and increasingly distrusted:

- 68% of users are dissatisfied with loyalty programs (Bond Brand Loyalty)
- 45% of millennials consider switching brands over data privacy concerns (McKinsey)
- Most loyalty points are trapped within closed ecosystems
- Users cannot transfer or monetize their achievements across services

Meanwhile, startups like Pollen ($150M) and Blackbird.xyz ($24M from a16z) highlight the demand for innovation in the space — but they offer closed platforms, not open standards.

## 3. Introducing UPAS (User Personal Achievement Standard): Open Reputation and Loyalty Protocol:

- **Open Architecture**: Non-expiring points architecture supporting cross-program transfers
- **Privacy-first**: Direct data exchange between users and businesses
- **Business-Ready**: Jurisdiction-agnostic design minimizing regulatory risks
- **Data Marketplace**: Enabling users to monetize anonymized purchase and preferences data
- **Decentralized Reputation**: Allowing businesses to segment audiences through valuable metrics without data leaks


## 4. Use Case and Basic explanation

Sarah is a regular customer who shops at her favorite café and a nearby organic store. Normally, her rewards stay locked within each store. With UPAS:

- She receives a credential from the café
- The loyalty canister awards her points
- Her portable reputation improves
- The organic store offers her custom deals based on her verified loyalty profile

3tale is a loyalty platform built on top of UPAS that expands this concept into a gamified ecosystem:

- Reputation Wallet with a shared user identity
- Modular subnets per country (localized rules, partners, UX)
- Gamification and social mechanics
- Support for small businesses to issue verifiable achievements


### UPAS Core Components

UPAS creates a unified loyalty standard through four main components:

1. **Store Entity**
   - Businesses can create their digital presence
   - Issue verifiable credentials for purchases
   - Define reward schemes and special offers
   - Manage employee access through delegated keys

2. **User Entity**
   - Single digital identity for all loyalty programs
   - Privacy-preserved purchase history
   - Portable reputation across businesses
   - Control over data sharing preferences

3. **Loyalty Canister**
   - Manages point distribution and tracking
   - Processes achievement credentials
   - Calculates reputation scores
   - Handles cross-program point transfers

4. **Exchange Canister**
   - Centralized point of fiat-to-token exchange
   - Controlled by licensed financial entity
   - Compliant with financial regulations
   - Handles point redemption and fiat settlements
   - Keeps loyalty points separate from cryptocurrency regulations
   - Enables businesses to operate within traditional financial frameworks

For example, when Sarah makes a purchase:
1. The store issues a credential to her UPAS identity
2. The loyalty canister automatically calculates and awards points
3. Her reputation score updates based on the purchase
4. Other participating stores can offer personalized rewards based on her verified shopping patterns
5. When redeeming points, the Exchange Canister handles the conversion to real-world value without cryptocurrency complications

This system benefits all parties:
- **Users** gain a unified loyalty experience with portable benefits
- **Businesses** access verified customer data and can offer targeted incentives
- **Both** participate in a more efficient and valuable loyalty ecosystem
- **Regulatory Compliance** is maintained through the centralized exchange component

The UPAS protocol makes this possible through ICP's unique features, enabling secure credential issuance, privacy-preserved data sharing, and automated reward distribution without requiring users to manage multiple accounts or applications. The addition of the Exchange Canister ensures the system operates within existing financial regulations while maintaining the benefits of blockchain technology.


### Technical Advantages of ICP

UPAS leverages unique ICP features for developing decentralized loyalty programs: 

- **Canister Signatures**: Automatic certificate issuance for achievements
- **Native Account Abstraction**: Seamless experience for businesses and users
- **Reverse Gas**: Users don't pay for transactions - critical for mass adoption
- **HTTP Outcalls**: Direct integration with POS terminals and CRM systems
- **Built-in Identity**: Native decentralized infrastructure layer
- **High Performance**: Scalable architecture with low transaction costs

This combination of features makes ICP the ideal foundation for implementing a universal standard for digital achievements and reputation, positioning it as the backbone for next-generation loyalty solutions.

---

## Interaction Specifications & Software Requirements

While UPAS provides the backend infrastructure on ICP, successful implementation requires specific frontend applications and additional software components. This section outlines the recommended specifications for a complete loyalty system implementation.

### Identity Wallet Requirements

The user-facing wallet application should provide:

1. **Secure Key Management**
   - Encrypted private key storage using platform-specific secure storage (Apple/Android cloud)
   - User-friendly key recovery without exposing seed phrases
   - Support for multiple identity profiles (separate personal/business achievements)

2. **Blockchain Integration**
   - Real-time point balance display
   - Transaction history tracking
   - Credential management and viewing
   - Achievement progress monitoring

3. **Privacy Features**
   - Selective credential disclosure
   - Encrypted storage of purchase history
   - Control over data sharing preferences
   - Anonymous credential acceptance options

4. **User Experience**
   - QR code scanning for desktop interactions
   - Push notifications for transaction approval
   - Achievement progress tracking
   - Personalized reward recommendations

### Business Integration Components

Businesses need to implement several components for successful UPAS integration:

1. **Backend Integration Library**
   - Secure private key management for credential signing
   - Point distribution handling
   - Credential issuance functionality
   - Transaction verification methods
   - API integration with existing POS/CRM systems

2. **Frontend Widget**
   - Mobile app deep linking support
   - QR code generation for desktop users
   - Point redemption interface
   - Credential display and verification
   - User authentication flow

### Interaction Flow Specifications

A typical transaction follows this flow:

1. **Initial Connection**
   - User visits participating store's website/payment page
   - Store displays available point earning/redemption options
   - User connects via mobile app or QR code

2. **Transaction Processing**
   - Store presents point earning opportunities and bonus conditions
   - User approves connection through identity wallet
   - Store verifies relevant reputation credentials
   - Points are calculated based on purchase and reputation

3. **Post-Purchase Flow**
   - Store issues purchase credentials to user's address
   - User receives notification to accept credentials
   - Points are automatically distributed
   - New achievements are calculated and issued

4. **Point Redemption**
   - Business initiates point redemption request
   - Exchange Canister processes conversion
   - Store receives fiat settlement
   - Transaction records are updated

### Security Recommendations

1. **Private Key Management**
   - Secure storage of business signing keys
   - Delegated key system for employee access
   - Regular key rotation policies
   - Backup and recovery procedures

2. **Data Privacy**
   - Encrypted storage of customer data
   - Minimal collection of personal information
   - Transparent data usage policies
   - Secure credential transmission

3. **Integration Security**
   - API authentication and authorization
   - Rate limiting and abuse prevention
   - Audit logging
   - Error handling and recovery procedures

This specification provides a framework for developers to build user-friendly applications while maintaining the security and privacy features core to the UPAS protocol. Implementations may vary based on specific business needs, but should maintain these core interaction patterns to ensure compatibility across the ecosystem.

# Bitcoin Hackerspace Network | BitHackNet
![BitcoinHackerspaceNetwork](./img/BitcoinHackerspaceNetwork.png)

## Summary
Bitcoin Hackerspace Network (BitHackNet) is a self-sovereign movement to connect bitcoin-focused hackerspaces across the globe to form a decentralized network 
of bitcoin-focused, physical spaces. The specific goals of these hackerspaces vary, but the first principle that all are built upon is the idea of "building builders."
We believe that bitcoiners from near and far should be able to enjoy the feeling of their local bitcoin community while on the road. BitHackNet strives to achieve this goal by providing its member hackerspacers with the technology to easily onboard members in a cryptographically verifiable way.

Digitally verifiable credentials provide the bitcoin hackerspace network with the ability to move freely between hackerspaces in different countries and cities within BitHackNet. A bitcoiner wanting to become a member of BitHackNet would contact a hackerspace participating in the network (typically one that is closest to them) and ask about onboarding. Generally speaking, "onboarding" requires selecting a memebership, paying an invoice and acquiring a BitHackNet credential from an issuer. Users with a BitHackNet credential enjoy various memeber benefits at any of the participating hackerspaces. Additionally, hackerspace organizers can rest assured that the out-of-towner standing in front of them has been onboarded by a network hackerspace they trust. In this way, we can provide easier access to hackerspaces for bitcoiners, provide more members and more revenue for hackerspaces, and provide the industry and world with more builders.

## Goals
1. Publish open-source documentation to allow future hackerspaces the ability to onboard themselves (self-sovereign) into the network
2. Define clear business requirements with resepect to cross-hackerspace, intra-network memebership benefits
    - [ ] Define business model
    - [ ] Define cost structure and rev share / split
    - [ ] Define benefits to members from one hackerspace to another
3. Define clear technical requirements (functional and non-functional) from the business requirements
4. Implement definitions from biz/tech reqs
    - [ ] Define JSON schema representing a hackerspace's belonging to / membership to the network
    - [ ] Define JSON schema for members + memberships
    - [ ] Define protocol for storing and retrieving JSON schema
    - [ ] Define protocol for proof request/response (request proof of membership/response with proof)
    - [ ] Implement TBD primitives building a "one-click" hackerspace technical repo
    - [ ] Research alternative protocols and interoperability with SSI/DIDs (e.g. nostr)
5. Onboard all bitcoin hackerspaces globally that want to participate

## Hackerspace Credential Schema Suggestion (HACS)
Below are proposed credential schemas for the Bitcoin Hackerspace Network. If you have improvements or suggestions, please feel free to fork and submit a PR.

|    Version    |     Credentials & Schemas      |     Title     |                      Description                                                                              |
|---------------|--------------------------------|---------------|---------------------------------------------------------------------------------------------------------------|
| [1](./1.0.0/) |  [temp](./1.0.0/schema.json)   |  Temp Schema  |  Defined large, nested schema as a catch all to get something completed for iterative sake                    |
| [2](./2.0.0/) |  [base](./2.0.0/schemas/)      |  Base Schemas |  Broke out each entity into its own credential, plan to reference parent child relationships beteween schemas |

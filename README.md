# Bitcoin Hackerspace Network
[![BitcoinHackerspaceNetwork](./img/BitcoinHackerspaceNetwork.png)](https://bitcoin.hackerspace.network)

## Summary
Bitcoin Hackerspace Network (BitHackNet) is a self-sovereign movement to connect bitcoin-focused hackerspaces across the globe to form a decentralized network 
of bitcoin-focused, physical spaces. The specific goals of these hackerspaces vary, but the first principle that all are built upon is the idea of "building builders."
We believe that bitcoiners from near and far should be able to enjoy the feeling of their local bitcoin community while on the road.

BitHackNet strives to achieve this goal by providing its member hackerspacers with the technology to easily onboard members in a cryptographically verifiable way. Digitally verifiable credentials provide the bitcoin hackerspace network with the ability to move freely between hackerspaces in different countries and cities within BitHackNet. A bitcoiner wanting to become a member of BitHackNet would contact a hackerspace participating in the network (typically one that is closest to them) and ask about onboarding.

Generally speaking, "onboarding" requires selecting a memebership, paying an invoice and acquiring a BitHackNet credential from an issuer. Users with a BitHackNet credential enjoy various memeber benefits at any of the participating hackerspaces. Additionally, hackerspace organizers can rest assured that the out-of-towner standing in front of them has been onboarded by a network hackerspace they trust. In this way, we can provide easier access to hackerspaces for bitcoiners, provide more members and more revenue for hackerspaces, and provide the industry and world with more builders.

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

## Hackerspace Credential and Key Schema Suggestion (HaCKS)*
_*HaCKS is a temp working name, looking for feedback on good names for submitting improvements to the schemas used for various cerdentials and entity interactions_

What should we can improvement proposals submitted to BitHackNet?
1. Hackerspace Credential and Key Schema Suggestions (HaCKSs, HaCKS, HACKS)
2. HackNet Improvement Proposals (HIPs)
3. Schema Improvement Proposals for Hackerspace Entity Network (SIPHENs)
4. Design of Credential Schemas (DOCS) for Bitcoin Hackerspaces
5. Bitcoin Third Place Network Improvement Proposals (BTPNIP)
6. Bitcoin Hackerspace Network Improvement Proposals (BitHackNIP)
7. Good Recommendations and Proposals for Hackerspaces (GRaPHs)
8. Hackerspace Identity Credential and Key Schema Suggestion (HICKS)*
9. Hackerspace Identity Schema Suggestion (HISS)*

Below are proposed credential schemas for the Bitcoin Hackerspace Network. If you have improvements or suggestions, please feel free to fork and submit a PR.

|        Version       |          Documentation         |     Title     |     Author    |
|----------------------|--------------------------------|---------------|---------------|
| [0](./hacks-0000.md) |   [hacks-0000](./hacks-0000)   | HaCKS Process |  Bryan Nonni  |
| [1](./hacks-0001.md) |   [hacks-0001](./hacks-0001/)  |  Temp Schema  |  Bryan Nonni  |
| [2](./hacks-0002.md) |   [hacks-0002](./hacks-0002/)  |  Base Schemas |  Bryan Nonni  |

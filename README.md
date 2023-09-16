# Bitcoin Hackerspace Network
[![bitcoin-hackerspace-network-header-img](./graph-0000/header.png)](https://bitcoin.hackerspace.network)

## BitHackNet Summary
Bitcoin Hackerspace Network (BitHackNet) is a self-sovereign movement connecting bitcoin-focused hackerspaces across the globe to form a decentralized network 
of physical bitcoin-focused spaces. The specific goals of these hackerspaces vary, but the first principle that all are built upon is the idea of building builders.

BitHackNet strives to achieve this goal by providing its members and member hackerspaces with the technology to easily onboard new members in a cryptographically verifiable way. Self-sovereign identity verifiable credentials is part of the solution while a communications protocol provides the other part. Together, these two technology primitives can be used to issue credentials to bitcoiners wanting to join their local hackerspace and gain access to the entirty of BitHackNet. To become a member of BitHackNet, contact a hackerspace participating in the network (typically one that is closest to you) and ask about onboarding.

Generally speaking, "onboarding" requires selecting a memebership, paying an invoice and acquiring a BitHackNet credential from an issuer. In ideal case, the onboarding hackerspace is also the issuer running their own ssi-service server; however, an alternative is to have another hackerspace in network do the issuing on their behalf and either store it with the proxy issuer or with the onboarder. The idea is that people with a BitHackNet credential will be able to enjoy various benefits at any of the participating hackerspaces. The exact details of those benefits may vary pending on location and must be designed collaboratively by the network members. That is one of the goals of this repository. Additionally, hackerspace organizers can rest assured that the out-of-towner standing in front of them has been onboarded by a network hackerspace they trust. In this way, we can provide easier access to hackerspaces for bitcoiners, provide more members and more revenue for hackerspaces, and provide the industry and world with more builders.

## BitHackNet Goals
1. Connect bitcoin hackerspaces into a global network
2. Provide value to hackerspace members
3. Provide support to hackerspaces
4. Build builders
5. Change the world, together

## Purpose
The main purpose of this repo is to provide an easy and efficient way for the community to collaborate on best practices, design and implementation of the various parts of the hackerspace network. 
### General Information
1. Best practices for onboarding new hackerspaces to network and members to hackerspaces (operations)
2. Best practices for maintaining profitability, scalability and collboration (business)
3. Best practices for implementing and improving the technical specification.
4. Documents to explain technical design and implementation
5. GRAPHs

### Technical Documentation
1. Publish open-source documentation to allow future hackerspaces the ability to onboard themselves (self-sovereign) into the network
2. Define best practices for sustainable business models between the hackerspaces and maintain each space's respective success metric (i.e. profit, non-profit, low costs, break even, etc.)
    - [ ] Define intra-network memebership benefits on a space-by-space basis
    - [ ] Determine how that is represented in a credential and attached to a member credential
    - [ ] Define cost structure and rev share / split on a space-by-space basis
3. Design and document technical parts (schemas, protocols, etc.)
    - [ ] JSON schema to represent hackerspaces and their membership to BitHackNet
    - [ ] JSON schema to represent members and their membership to their onboarding / issuing hackerspace
    - [ ] JSON schema to represent memberships and the specific benefits available to the holding members
    - [ ] Protocol for issuing valid credentials to hackerspaces and memebers
    - [ ] Protocol for storing and retrieving JSON schemas and credentials
    - [ ] Protocol for presentation (by the holder) and verification of credentials
4. Implement technical design as an open source repo functioning like a hackerspace "toolbox"
    - [ ] SSI stack: implement SSI primitives building a "one-click" solution using DIDs, VCs and DWNs
    - [ ] Alt stack: design and implement the system with alternative protocols (e.g. nostr)
    - [ ] Interoperability: design and implement ways to interoperate these tech stacks
5. Onboard all bitcoin hackerspaces globally that want to participate

## Guidelines and Resources to Advance Protocols for Hackerspaces (GRAPH)
_*GRAPH is a temp working name, looking for feedback on good names for submitting improvements to the schemas used for various cerdentials and entity interactions. Possible alternatives [here](./graph-0000.md)_

Below are proposed credential schemas for the Bitcoin Hackerspace Network. If you have improvements or suggestions, please feel free to fork and submit a PR.

|        Version       |          Documentation         |     Title     |     Author    |
|----------------------|--------------------------------|---------------|---------------|
| [0](./graph-0000.md) |   [graph-0000](./graph-0000)   | GRAPH Process |  Bryan Nonni  |
| [1](./graph-0001.md) |   [graph-0001](./graph-0001/)  |  Temp Schema  |  Bryan Nonni  |
| [2](./graph-0002.md) |   [graph-0002](./graph-0002/)  |  Base Schemas |  Bryan Nonni  |

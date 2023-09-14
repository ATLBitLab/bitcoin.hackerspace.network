![image](https://github.com/ATLBitLab/initiative-bitcoin-hackerspace-network/assets/19941207/b1bdfd51-393b-4e67-9e7f-4742c8dcfd47)

## Summary
Initiative: Bitcoin Hackerspace Network is a self-sovereign movement to connect bitcoin-focused hackerspaces across the globe into a decentralized network
of physical bitcoin-only locations. Doing so allows bitcoiners from near and far to onboard near to them and enjoy a community far from them.
By onboarding to a local hackerspace in init:**bithacknet**, users can enjoy the benefits of a safe and bitcoin-focused communtity in a number of countries around the world. Alternatively, hackerspace leaders can rest assured that the out-of-towner standing in front of them has been vetted and onboarded by a network hackerspace they trust. In this way, we can lower the barriers to entry for all who want to learn how to build and fulfill the promise of local, community-led bitcoin education and specifically that of bitcoin hackerspaces - building more builders.

## Goals
1. Publish open-source documentation to allow future hackerspaces the ability to onboard themselves (self-sovereign) into the network
2. Define clear business requirements with resepect to cross-hackerspace, intra-network memebership benefits
   - define business model
   - define cost structure and revenue shared / split
   - define benefits to members from one hackerspace to another
3. Define clear technical requirements (functional and non-functional) from the business requirements
4. Implement definitions from biz/tech reqs
   - define JSON schema representing a hackerspace's belonging to / membership to the network
   - define JSON schema for members + memberships
   - define protocol for storing and retrieving JSON schema
   - define protocol for proof request/response (request proof of membership/response with proof)
   - implement TBD primitives building a "one-click" hackerspace technical repo
   - research alternative protocols and interoperability with SSI/DIDs (e.g. nostr)
5. Scale all business and technical resources to the world onboarding all bitcoin hackerspaces


## Schemas
Below are various schemas for credentials that can be signed by an issuing key and sent to a receiving key who holds the credential.
Later, the holder can present the credential as proof of their membership to a hackerspace in the network.
- [Current Working Schema: Network, Membership, Member](./schemas/current.json)
- [Network Schema](./schemas/network.json)
- [Hackerspace Schema](./schemas/hackerspace.json)
- [Membership Schema](./schemas/membership.json)
- [Member Schema](./schemas/member.json)
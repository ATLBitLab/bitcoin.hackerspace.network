![image](https://github.com/ATLBitLab/bitcoin.hackerspace.network/assets/19941207/138be3af-8af1-4c06-93a5-9f8aefed7bcb)

## Summary
Bitcoin Hackerspace Network (or BTCHackNet) is a self-sovereign movement to connect bitcoin-focused hackerspaces across the globe to form a decentralized network
of physical bitcoin-only spaces meant for building builders. We believe that bitcoiners from near and far should be able to enjoy the feeling of their local bitcoin community while on the road. BTCHackNet strives to achieve this goal by providing onbaorded members the ability to move freely between countries, cities and bitcoin hackerspaces in BTCHackNet. A bitcoiner wanting to become a member of BTCHackNet would contact a hackerspace participating in BTCHackNet that is closest to them and onboard. Onboarding, generally speaking, means selecting a memebership tier, paying the Lightning invoice and being issued a credential representing membership to BTCHackNet. Users with credentials inside BTCHackNet can enjoy various memeber benefits at any of the participating hackerspaces. Additionally, hackerspace organizers can rest assured that the out-of-towner standing in front of them has been onboarded by a network hackerspace they trust. In this way, we can lower the barriers of entry for all who want to learn how to build and drive closer to our goal: building more builders.

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

# Bitcoin Hackerspace Member VC

## Summary
The goal of this document is to define a spec for a Self-Sovereign Identity Verifiable Credential schema to represent a member of a Bitcoin hackerspace.
This member VC represents the holder and their membership to the issuing hackerspace and the list of participating hackerspaces.
Members holding one of these credentials have been verified by the issuer and are afforded certain rights, privileges, entitlements and/or benefits, such as:
  - access to the issuing hackerspace
  - access to hackerspaces in the network as defined in the VC
  - access to amenities in those hackerspaces

## Schema
```json
{
  "name": "Bitcoin Hackerspace Member Credential",
  "issuer": "did:ion:EiDf5lBVA9z_Alm7ppaPY2ee7epUTspFiTYkz2eLW_kVzw",
  "verificationMethodId": "did:ion:EiDf5lBVA9z_Alm7ppaPY2ee7epUTspFiTYkz2eLW_kVzw#did:ion:EiDf5lBVA9z_Alm7ppaPY2ee7epUTspFiTYkz2eLW_kVzw"
  "description": "Credential representing a bitcoin hackerspace member, membership to the issuing hackerspace and membership to network of hackerspaces",
  "schema": {
    "$schema": "https://json-schema.org/draft/2020-12/schema",
    "emailAddress": {
      "type": "string",
      "format": "email"
      }
  }
}
```

#### Data Types
```typescript
  type Bitcoin_Hackerspace_Member_VC_Schema = {
    holder: {
      name: String;
      email: String;
      website: String;
      telegram: String;
      x: String;
      npub: String;
      nip5: String;
    };
    network: {
      name: String;
      country: String;
      states: Array<String>;
      cities: Array<String>;
      organizations: Array<String>;
    };
    membership: {
      title: String;
      tier: Number;
      description: String;
      benefits: Array<String>;
    };
  };
```

## Example

```js
  const MemberVC = {
    holder: {
      name: "abbot",
      email: "abbot@atlbitlab.com",
      website: "https://abbot.atlbitlab.com",
      telegram: "abbot",
      x: "abbot",
      npub: "npub123456...",
      nip5: "abbot@atlbitlab.com",
    },
    network: {
      name: "Federation of Bitcoin Hackerspaces",
      country: "US",
      states: ["georgia", "texas"],
      cities: ["atlanta", "austin"],
      organizations: ["atl bitlab", "pleblab"],
    },
    membership: {
      title: "Day Pass",
      tier: 0,
      description:
        "free day pass redeemable by the holder listed at any of the network organizations listed",
      benefits: [
        "wifi",
        "drinks",
        "snacks",
        "hot_desk",
        "conference_rooms",
        "alcohol",
      ],
    },
  };
```

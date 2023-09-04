# Bitcoin Hackerspace Membership VC

## Summary
The goal of this document is to define a spec for a Self-Sovereign Identity Verifiable Credential schema for membership to a Bitcoin hacker space or a network of Bitcoin hacker spaces.
Members holding one of these credentials have been verified by the issuer and are afforded certain rights, privileges, entitlements and/or benefits, such as:
  - access to the issuing hacker space
  - access to hacker spaces in the network defined in the VC
  - access to amenities in those hacker spaces

## Schema

```typescript
  type Bitcoin_Hackerspace_Membership_VC = {
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
  const member = {
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

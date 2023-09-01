# Bitcoin Hackerspace Membership VC

## Summary

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

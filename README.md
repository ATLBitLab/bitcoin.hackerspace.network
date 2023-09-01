# Bitcoin Hackerspace Membership VC

## Summary

## Schema

```typescript
type BTCHackerspaceMembershipVC = {
  name: String;
  contact: {
    email: String;
    telegram: String;
    twitter: String;
    nostr: {
      npub: String;
      nip5: String;
    };
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
    type: String;
    description: String;
    benefits: Array<String>;
  };
};
```

## Example

```json
{
  "holder": {
    "name": "abbot",
    "email": "abbot@atlbitlab.com",
    "website": "https://abbot.atlbitlab.com",
    "telegram": "abbot",
    "x": "abbot",
    "npub": "npub123456...",
    "nip5": "abbot@atlbitlab.com"
  },
  "network": {
    "country": "US",
    "states": ["georgia", "texas"],
    "cities": ["atlanta", "austin"],
    "name": "Federation of Bitcoin Hackerspaces",
    "organizations": ["atl bitlab", "pleblab"]
  },
  "membership": {
    "title": "Digital Nomad",
    "tier": 0,
    "type": "day pass",
    "description": "free day pass redeemable by the holder at any of the network participant locations",
    "benefits": [
      "wifi",
      "drinks",
      "snacks",
      "hot_desk",
      "conference_room",
      "beer"
    ]
  }
}
```

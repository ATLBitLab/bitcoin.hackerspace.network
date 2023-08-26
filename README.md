# Bitcoin Hackerspace Membership VC

## Summary


## Schema
```typescript
type BTCHackerspaceMembershipVC = {
    name: String
    contact: {
        email: String
        telegram: String
        twitter: String
        nostr: {
            npub: String
            nip5: String
        }
    },
    network: {
        name: String
        participants: Array<String>
    },
    membership: {
        tier: Number
        type: String
        description: String
        benefits: Array<String>
    }
}
```

## Example
```json
{
    "name": "pleb",
    "contact": {
        "email": "pleb@atlbitlab.com",
        "telegram": "pleb",
        "x": "pleb",
        "nostr": {
            "npub": "npub123456...",
            "nip5": "pleb@atlbitlab.com"
        }
    },
    "network": {
        "name": "federation of bitcoin hackerspace",
        "participants": ["atl bitlab", "pleblab"]
    },
    "membership": {
        "title": "Digital Nomad",
        "tier": 0,
        "type": "day pass",
        "description": "free day pass redeemable by the holder at any of the network participant locations",
        "benefits": ["wifi", "drinks", "snacks", "hot_desk", "conference_room", "beer"]
    }
}
```
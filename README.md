# Bitcoin Hackerspace Network Membership Credential

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
  "member": {
    "type": "object",
    "description": "Details about the member including name, contact information, website and socials.",
    "name": {
      "type": "string",
      "description": "The member's name."
    },
    "email": {
      "type": "string",
      "description": "The member's email."
    },
    "website": {
      "type": "string",
      "description": "website."
    },
    "telegram": {
      "type": "string",
      "description": "The member's telegram handle."
    },
    "x": {
      "type": "string",
      "description": "The member's X.com (f.k.a. Twitter) handle."
    },
    "npub": {
      "type": "string",
      "description": "The member's nostr npub."
    },
    "nip5": {
      "type": "string",
      "description": "The member's nostr nip5."
    }
  },
  "network": {
    "type": "object",
    "description": "Details about the hackerspace network that the issuer and member belongs.",
    "name": {
      "type": "string",
      "description": "The name of the network of hackerspaces that the issuer and member belong to."
    },
    "hackerspaces": {
      "type": "array",
      "description": "The hackerspaces participathing in the network that the member belongs to."
    },
    "countries": {
      "type": "array",
      "description": "The countries where the hackerspaces participating in the network are located."
    },
    "states": {
      "type": "array",
      "description": "The states where the hackerspaces participating in the network are located."
    },
    "cities": {
      "type": "array",
      "description": "The cities where the hackerspaces participating in the network are located."
    }
  },
  "membership": {
    "type": "object",
    "description": "Details about the membership to the network hackerspaces.",
    "issuer": {
      "type": "string",
      "description": "The name of hackerspace issuing the credential."
    },
    "title": {
      "type": "string",
      "description": "The membership title."
    },
    "tier": {
      "type": "number",
      "description": "The membership tier."
    },
    "description": {
      "type": "string",
      "description": "Any general information about the membership."
    },
    "benefits": {
      "type": "array",
      "description": "The amentities and benefits available to the membership tier."
    }
  }
}
```

## Example

```json
  {
    "member": {
      "name": "abbot",
      "email": "abbot@atlbitlab.com",
      "website": "https://abbot.atlbitlab.com",
      "telegram": "atl_bitlab_bot",
      "x": "atlbitlabbot",
      "npub": "npub1agq3p0xznd07eactnzv2lur7nd62uaj0vuar328et3u0kzjprzxqxcqvrk",
      "nip5": "abbot@atlbitlab.com",
    },
    "network": {
      "name": "Federation of Bitcoin Hackerspaces",
      "hackerspaces": ["ATL BitLab", "PlebLab"],
      "countries": ["United States of America"],
      "states": ["Georgia", "Texas"],
      "cities": ["Atlanta", "Austin"]
    },
    "membership": {
      "issuer": "ATL BitLab",
      "title": "Day Pass",
      "tier": 0,
      "description": "The Day Pass membership is redeemable for one free work day at any of the hackerspaces participating in the network.",
      "benefits": [
        "wifi",
        "coffee",
        "snacks",
        "hot desk",
        "conference rooms",
        "alcohol"
      ],
    },
  };
```

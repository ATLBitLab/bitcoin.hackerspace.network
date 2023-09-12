# the bitcoin hackerspace initiative

## Summary

The goal of this document is to define a schema for a Self-Sovereign Identity Verifiable Credential.

The credential represents a member, their membership to the issuing hackerspace, their membership and the issuer's membership to the bitcoin hackerspace initiative network. Members holding one of these credentials have been verified and onboarded into the network by the issuer and are afforded certain rights, privileges, entitlements and/or benefits, such as:

- access to the issuing hackerspace as defined in the schema
- access to network of hackerspaces as defined in the schema
- access to amenities at issuing hackerspace and network hackerspaces as defined in the schema

## Schema

```json
{
  "name": "bitcoin hackerspace member credential",
  "issuer": "did:key:z6MkhMe7QsyySXEQ6A8BJ1iaFAScNKaasZtmZ7ppsweovuDs",
  "verificationMethodId": "did:key:z6MkhMe7QsyySXEQ6A8BJ1iaFAScNKaasZtmZ7ppsweovuDs#z6MkhMe7QsyySXEQ6A8BJ1iaFAScNKaasZtmZ7ppsweovuDs",
  "description": "Credential representing a bitcoin hackerspace member, membership to the issuing hackerspace and membership to network of hackerspaces",
  "schema": {
    "$schema": "https://json-schema.org/draft/2020-12/schema",
    "type": "object",
    "properties": {
      "member": {
        "type": "object",
        "description": "Details about the member including name, contact information, website and socials.",
        "required": [
          "name",
          "email"
        ],
        "properties": {
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
            "description": "The member's website."
          },
          "telegram": {
            "type": "string",
            "description": "Member telegram handle."
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
        }
      },
      "membership": {
        "type": "object",
        "required": [
          "issuer",
          "title",
          "tier",
          "description",
          "benefits"
        ],
        "properties": {
          "issuer": {
            "type": "object",
            "description": "The details of hackerspace issuing the credential.",
            "required": [
              "website",
              "name",
              "country",
              "state",
              "city"
            ],
            "properties": {
              "website": {
                "type": "string",
                "description": "The website of the issuing hackerspace."
              },
              "name": {
                "type": "string",
                "description": "The name of the issuing hackerspace."
              },
              "country": {
                "type": "string",
                "description": "The country of the issuing hackerspace."
              },
              "state": {
                "type": "string",
                "description": "The state of the issuing hackerspace."
              },
              "city": {
                "type": "string",
                "description": "The city of the issuing hackerspace."
              }
            }
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
    },
    "network": {
      "type": "object",
      "description": "Details about the hackerspace network that the issuer and member belong to.",
      "required": [
        "name",
        "hackerspaces",
        "countries",
        "states",
        "cities"
      ],
      "properties": {
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
      }
    },
    "required": [
      "member",
      "membership",
      "network"
    ]
  }
}
```

## Credential

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
  "membership": {
    "issuer": {
      "website": "https://atlbitlab.com",
      "name": "ATL BitLab",
      "country": "United States of America",
      "state": "Georgia",
      "city": "Atlanta"
    },
    "title": "Day Pass",
    "tier": 0,
    "description": "This credential is redeemable for one free work day at any of the hackerspaces participating in the network.",
    "benefits": [
      "wifi",
      "coffee",
      "snacks",
      "hot desk",
      "conference rooms",
      "alcohol"
    ]
  },
  "network": {
    "name": "the bitcoin hackerspace initiative",
    "hackerspaces": [
      "ATL BitLab",
      "PlebLab"
    ],
    "countries": [
      "United States of America"
    ],
    "states": [
      "Georgia",
      "Texas"
    ],
    "cities": [
      "Atlanta",
      "Austin"
    ]
  }
}
```

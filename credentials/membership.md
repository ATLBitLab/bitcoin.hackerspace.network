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
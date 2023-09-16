```
HaCKS: 2
Title: Base Schemas
Status: Active
Author: Bryan Nonni <bryan@atlbitlab.com>
Created: 2023-09-06
License: CC0
```
## Abstract
This HaCKS proposes breaking out each entity from HaCKS 0001 into its own credential. The plan is to reference schemas inside issued credentials in a parent-child relationship. For example, every credential issued to a user from a hackerspace in this network will be of type HackerspaceMembership. This credential will point to a HackerspaceMember credential, and this HackerspaceMember credential will point to a NetworkHackerspace credential. NetworkHackerspace and HackerspaceMember credential schemas are more static and less likely to change, where as members may change their membership detials often. This way, we can avoid having to reissue 1 massive credential or 3-4 different credentials if things change for memebrs.

## Specification

TODO: Diagram

[NetworkHackerspace Schema](./hacks-0002/schemas/NetworkHackerspace.json)
[HackerspaceMembership Schema](./hacks-0002/schemas/HackerspaceMembership.json)
[HackerspaceMember Schema](./hacks-0002/schemas/HackerspaceMember.json)

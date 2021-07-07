# ChippIn Docs | Groups - Overview

The groups do not have any **admin** users. There is no heirarchy between group members to maintain trust. Any user can create a group and invite any user to join the group they are already a part of.

Each time a group is created, a new wallet is assigned to it. Members can pool-in money as they required and the **Rapyd Node SDK** provides all tools to transfer funds between users' and group's wallets.

## Models

### Group Model
The *Group Object* contians the follwoing:

| Attribute   |      Type      |  Description |
|----------|:-------------:|------|
| id | string | MongoDB-generated unique id. |
| name | string | Name of the group. |
| amount.upperLimit | Number | The restriction on total pool-in amount. |
| amount.current | Number | Current amount available in the group. |
| member.count |  Number | Number of group members. |
| ewalletId | string | Rapyd ewalletId |

The model can be found in `src/server/models/Group.js`.
 
### GroupMember Model
The *GroupMember Object* is used to store associations of each user and a group:

| Attribute   |      Type      |  Description |
|----------|:-------------:|------|
| id | string | MongoDB-generated unique id. |
| groupId | string | MongoDB-generated group id. |
| userId | string | MongoDB-generated user id. |
| ewalletId | string | Rapyd ewalletId. |

Read [Groups Usage](Groups/usage.md) complete implementation details involving Rapyd API.
# az-cli-cmds
## Cheat sheet of useful commands

List role assignment for a subscription

`az role assignment list --subscription 'subcritpion_id' --output json --query '[].{principalName:principalName, roleDefinitionName:roleDefinitionName, scope:scope}'`

List role assignment for a subscription for a user

`az role assignment list --all --include-inherited --assignee 'identity_address' --output json --query '[].{principalName:principalName, roleDefinitionName:roleDefinitionName, scope:scope}' --subscription 'subscription id' `

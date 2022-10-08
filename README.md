# az-cli-cmds
## Cheat sheet of useful commands

List role assignment for a subscription

`az role assignment list --subscription 'subcritpion_id' --output json --query '[].{principalName:principalName, roleDefinitionName:roleDefinitionName, scope:scope}'`

List role assignment for a subscription for a user

`az role assignment list --all --include-inherited --assignee 'identity_address' --output json --query '[].{principalName:principalName, roleDefinitionName:roleDefinitionName, scope:scope}' --subscription 'subscription id' `

List actions done on a subscription based on Activity Logs for the last 300 days

`az monitor activity-log list --output json --query '[].authorization.action' --start-time 2022-08-24 --offset 300d`

List group membership for a user

`az ad user get-member-groups --id`

# az-cli-cmds
Cheat sheet of useful commands

List role assignment for a subscription

<sub> az role assignment list --subscription 'subcritpion_id' --output json --query '[].{principalName:principalName, roleDefinitionName:roleDefinitionName, scope:scope}' </sub>

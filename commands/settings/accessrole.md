# `+accessrole` command
Sets a role that people have to have to use the bot.

## Syntax
```
++accessrole <role>
```
Parameter | Required | Type               | Description
----------|----------|--------------------|--------------------------------------------------
role      | Yes      | role (name or role id) | The prefix you want to set. If set to `disable`, the prefix will go back to the default value of `+`

### Example
```
++accessrole Trusted
```
This command will set the access role to Trusted, only allowing people with the Trusted role to use the bot.

## Permission
This command require the `settings.accessrole` permission node.
```
+perms add Administrators settings.accessrole
```

See the [permissions page](/permissions.md) for more informations.

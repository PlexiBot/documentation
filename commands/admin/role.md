# `role` command
This command allows you to add or remove roles from a member or a group of members of your server.
By adding the rolename into the `member` field, the group of members assigned to the role will be aimed at.

## Syntax
```
+role <action> <member> <role> [reason]
```
Parameter | Required |        Type        | Description
----------|----------|--------------------|--------------------------------------------------
action    | Yes      | option (add/remove)| The action you want to execute.
member    | Yes      | member/rolename    | The member or the group of members you want to assign or remove roles from.
role      | Yes      | text (rolename)    | The role you want to assign or remove from a member or a group of members.
reason    | No       | text               | The reason that will be logged in the Discord's Audit Log.

### Example
```
+role add luke Kids No NSFW!
```
This command will assign the role `Kids` to the member `luke` with the reason `No NSFW!`.

## Permission
This command requires the `admin.role` permission node.
```
+perms add Moderators admin.role
```
As a safeguard, this command will also require you to have the `Manage roles` Discord's permission.

See the [permissions page](/permissions.md) for more informations.

# `+kick` command
This command allow you to kick a member from your server.

## Syntax
```
++kick <member> [reason]
```
Parameter | Required | Type               | Description
----------|----------|--------------------|--------------------------------------------------
member    | Yes      | member (@mention)  | The member to ban. It should be in your server.
reason    | No       | text               | The reason that will be logged with the ban and in the Discord's Audit Log. If you have a log channel set (see [`+log`](/commands/settings/log.md)), the reason may be also logged in this channel.

### Example
```
++kick @RoleBreaker#0420 Breaking the rules.
```
This command will kick the user `RoleBreaker#0420` with the reason `Breaking the rules.`

## Permission
This command require the `admin.kick` permission node.
```
+perms add Moderators admin.kick
```
As a safeguard, this command will also require you to have the `Kick member` Discord's permission.

See the [permissions page](/permissions.md) for more informations.

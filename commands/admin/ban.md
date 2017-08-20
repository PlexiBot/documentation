# `+ban` command
This command allow you to ban a member from your server, temporarily or permanently.

## Syntax
```
+ban <member> [days] [reason]
```
Parameter | Required |        Type        | Description
----------|----------|--------------------|--------------------------------------------------
member    | Yes      | member (@mention)  | The member to ban. It should be in your server.
days      | No       | number             | The number of days after which the bot will be lifted. If not provided or set to `0`, this feature will be disabled.
reason    | No       | text               | The reason that will be logged with the ban and in the Discord's Audit Log. If you have a log channel set (see [`+log`](/commands/settings/log.md)), the reason may be also logged in this channel.

### Example
```
+ban @BadUser#5429 15 Bad guy
```
This command will ban the user `BadUser#5429` for `15` days with the reason `Bad guy`.

## Permission
This command require the `admin.ban` permission node.
```
+perms add Moderators admin.ban
```
As a safeguard, this command will also require you to have the `Ban member` Discord's permission.

See the [permissions page](/permissions.md) for more informations.

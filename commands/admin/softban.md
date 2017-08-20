# `+softban` command
This command allow you to kick a member from your server and removing its messages posted in the last 7 days.
That works by banning the user (to remove the messages), then unbanning it just after (this operation is often called a `softban`).

## Syntax
```
+softban <member> [reason]
```
Parameter | Required |        Type        | Description
----------|----------|--------------------|--------------------------------------------------
member    | Yes      | member (@mention)  | The member to kick. It should be in your server.
reason    | No       | text               | The reason that will be logged in the Discord's Audit Log. If you have a log channel set (see [`+log`](/commands/settings/log.md)), the reason may be also logged in this channel.

### Example
```
+softban @Spammer#5429 Spamming
```
This command will kick the user `Spammer#5429` with the reason `Spamming` and removes its messages posted in the last 7 days.

## Permission
This command require the `admin.softban` permission node.
```
+perms add Moderators admin.softban
```
As a safeguard, this command will also require you to have the `Kick member` Discord's permission.

See the [permissions page](/permissions.md) for more informations.

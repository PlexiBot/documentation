# `+mute` command
This command allow you to mute a user from your server.
That works by creating a role called `VexeraMuted` with permissions override to remove the `Send Messages` permission on every channels.
This role is then assigned to muted users.

## Syntax
```
+mute <member> [reason]
```
Parameter | Required |        Type        | Description
----------|----------|--------------------|--------------------------------------------------
member    | Yes      | member (@mention)  | The member to mute. It should be in your server.
reason    | No       | text               | The reason that will be logged in the Discord's Audit Log. If you have a log channel set (see [`+log`](/commands/settings/log.md)), the reason may be also logged in this channel.

### Example
```
+mute @Troll#5429 Trolling
```
This command will mute the user `Troll#5429` with the reason `Trolling` until the `VexeraMuted` role is removed.

## Permission
This command require the `admin.mute` permission node.
```
+perms add Moderators admin.mute
```
As a safeguard, this command will also require you to have the `Voice mute member` Discord's permission.

See the [permissions page](/permissions.md) for more informations.

## A note about the `VexeraMuted` role
This role is created the first time you mute a user. A permission override in every channels of your server is then created to remove the `Send Messages` permission.
The role should be updated automatically when you create a new channel.
If the role happens to be broken on your server, you can force Vexera to regenerate it by deleting (or renaming) the role and applying a new mute.

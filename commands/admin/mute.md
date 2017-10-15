# `+mute` command
This command allows you to mute a user from your server.
That works by creating a role called `Muted` with permissions override to remove the `Send Messages` permission on every channel.
This role is getting assigned to muted users.

## Syntax
```
+mute <member> [reason]
```
Parameter | Required |        Type        | Description
----------|----------|--------------------|--------------------------------------------------
member    | Yes      | member (@mention)  | The member to mute. It should be in your server.
reason    | No       | text               | The reason that will be logged in the Discord's Audit Log.

### Example
```
+mute @Troll#5429 Trolling
```
This command will mute the user `Troll#5429` with the reason `Trolling` until the `Muted` role is removed.

## Permission
This command requires the `admin.mute` permission node.
```
+perms add Moderators admin.mute
```
As a safeguard, this command will also require you to have the `Voice mute member` Discord's permission.

See the [permissions page](/permissions.md) for more informations.

## A note about the `Muted` role
This role is created the first time you mute a user. A permission override in every channel of your server is then created to remove the `Send Messages` permission.
The role should be updated automatically when you create a new channel.

If the role happens to be broken on your server, you can force Vexera to regenerate it by deleting (or renaming) it and applying a new mute.
Please note that after regenerating the role, you should remute all previously muted users.

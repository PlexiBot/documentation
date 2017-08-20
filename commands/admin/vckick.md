# `+vckick` command
This command allow you to kick a member from a voice channel.

## Syntax
```
+vckick <member> [reason]
```
Parameter | Required | Type               | Description
----------|----------|--------------------|--------------------------------------------------
member    | Yes      | member (@mention)  | The member to kick. It should be connected in a voice channel.
reason    | No       | text               | The reason that will be logged in the Discord's Audit Log. If you have a log channel set (see [`+log`](/commands/settings/log.md)), the reason may be also logged in this channel.

### Example
```
+vckick @Yeller#0420 YELL IN THE VOICE CHAT
```
This command will kick the user `Yeller#0420` with the reason `YELL IN THE VOICE CHAT`.

## Permission
This command require the `admin.vckick` permission node.
```
+perms add Moderators admin.vckick
```
As a safeguard, this command will also require you to have the `Kick member` Discord's permission.

See the [permissions page](/permissions.md) for more informations.

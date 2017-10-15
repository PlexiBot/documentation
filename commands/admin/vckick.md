# `+vckick` command
This command allows you to kick a member from a voice channel. That works by creating a voice channel called `voicekick`, 
moving the member to it and deleting it just after.

## Syntax
```
+vckick <member> [reason]
```
Parameter | Required | Type               | Description
----------|----------|--------------------|--------------------------------------------------
member    | Yes      | member (@mention)  | The member to kick. It should be connected to a voice channel.
reason    | No       | text               | The reason that will be logged in the Discord's Audit Log.

### Example
```
+vckick @Yeller#0420 YELL IN THE VOICE CHAT
```
This command will kick the user `Yeller#0420` *from the voice channel* with the reason `YELL IN THE VOICE CHAT`.

## Permission
This command requires the `admin.vckick` permission node.
```
+perms add Moderators admin.vckick
```
As a safeguard, this command will also require you to have the `Kick member` Discord's permission.

See the [permissions page](/permissions.md) for more informations.

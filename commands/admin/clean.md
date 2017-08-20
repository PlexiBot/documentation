# `+clean` command
This command allow you to clean messages from a channel.

## Syntax
```
+clean [amount=10] [user]
```
Parameter | Required | Type               | Description
----------|----------|--------------------|--------------------------------------------------
amount    | No       | number             | The amount of messages to remove. If not set, default to `10`.
user      | No       | username (text)    | Removes only messages from this user. If not set, removes messages from all users.

### Examples
```
+clean 100
```
This command will remove the last `100` messages in the current channel.

-----
```
+clean 100 luke
```
This command will remove the last `100` messages posted by `luke` in the current channel.

## Permission
This command require the `admin.clean` permission node.
```
+perms add Administrators admin.clean
```
As a safeguard, this command will also require you to have the `Manage messages` Discord's permission in the target channel.

See the [permissions page](/permissions.md) for more informations.

## Limitations
Due to a limitation with the Discord API to prevent abuses, this command cannot remove messages older than 14 days.

If you want to clear a channel with an extensive messages history, it's better to remove and recreate the channel.

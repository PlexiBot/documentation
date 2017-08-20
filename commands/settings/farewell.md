# `+farewell` command
This command sets a message for when a user leaves the server.

## Syntax
```
++farewell <channel> [text]
```
Parameter | Required | Type               | Description
----------|----------|--------------------|--------------------------------------------------
channel   | Yes      | channel (#mention) | The channel you want the farewell message to appear in.
text      | No       | string             | The text that you want to appear. You can use `%mention%` and `%server%` in this string.

### Example
```
++farewell #general %username% left %server%... bye bye %username%...
```
This command will send `luke left <your server>... bye bye luke..` to `#general` when luke leaves your server.

## Permission
This command require the `settings.farewell` permission node.
```
+perms add Administrators settings.farewell
```

See the [permissions page](/permissions.md) for more informations.

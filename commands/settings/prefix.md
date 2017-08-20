# `+prefix` command
This command allow you to change the prefix in which Vexera responds with.

## Syntax
```
+prefix <prefix>
```
Parameter | Required | Type               | Description
----------|----------|--------------------|--------------------------------------------------
prefix    | Yes      | string             | The prefix you want to set. If set to `disable`, the prefix will go back to the default value of `+`

### Examples
```
+prefix =
```
This command will set the prefix to `=`

```
+prefix disable
```
This command will disable the custom prefix and set the prefix to the default value of `+`

## Permission
This command require the `settings.prefix` permission node.
```
+perms add Administrators settings.prefix
```

See the [permissions page](/permissions.md) for more informations.

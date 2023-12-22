# MyPlugin

## 📑 Features

- Be a template for your own plugin
- Store the last connection time of a player
- Store the number of death of a player

## 🔑 Permissions

* `myplugin.admin` - Allows player to use the **/myplugin** command

## 📝 Commands

* `myplugin help` - Displays some help

## ⚙️ Configuration

Default configuration:

```json
{
  "Default Chat Avatar (steamId)": 0
}
```

## 🏳️ Localization

Default English localization:

```json
{
  "PluginMissing": "The plugin \"SomePlugin\" was not found. Check on UMod: https://umod.org/plugins/someplugin",
  "NoPermission": "You are not allowed to run this command!",
  "HelpMessage": "Some useful help!",
  "UnknownCommand": "Unknown command!"
}
```

## 🪝 Hooks

```csharp
DateTime? GetLastConnectionTime(ulong userId)
// Return the last connection time (DateTime?) of a player or null if the player is not found

int? GetNumberOfDeath(ulong userId)
// Return the number (int?) of death of a player or null if the player is not found
```

## 🖼️ Credits

* **[YourName](https://github.com/YourName)** - Author
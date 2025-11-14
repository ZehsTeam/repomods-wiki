# Getting Started with REPOLib (C#)

This page assumes you have a C# project setup for R.E.P.O. modding. If not, first follow the guide in [Developing Mods](../../develop.md).

## Installation

Reference [REPOLib](https://www.nuget.org/packages/Zehs.REPOLib) in your project's `.csproj` file:

```xml
<ItemGroup>
  <PackageReference Include="Zehs.REPOLib" Version="3.*" />
</ItemGroup>
```

Add REPOLib as a dependency to your plugin class:

```c#
[BepInDependency(REPOLib.MyPluginInfo.PLUGIN_GUID)]
```

```c#
[BepInPlugin("You.YourMod", "YourMod", "1.0.0")]
[BepInDependency(REPOLib.MyPluginInfo.PLUGIN_GUID)]
public class YourMod : BaseUnityPlugin
{
    // ...
}
```

# Registering Shop Items with REPOLib

Registering an item:

```c#
using REPOLib.Objects.Sdk;

private void awake()
{
    REPOLib.BundleLoader.LoadBundle("your_assetbundle_file_path", assetBundle =>
    {
        // The type ItemContent is from REPOLib.Objects.Sdk
        var item = assetBundle.LoadAsset<ItemContent>("your_item_content");
        REPOLib.Modules.Items.RegisterItem(item);
    });
}
```

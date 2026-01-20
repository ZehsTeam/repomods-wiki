# Registering Enemies with REPOLib

Registering an enemy:

```c#
using REPOLib.Objects.Sdk;

private void Awake()
{
    REPOLib.BundleLoader.LoadBundle("your_assetbundle_file_path", assetBundle =>
    {
        // The type EnemyContent is from REPOLib.Objects.Sdk
        var enemyContent = assetBundle.LoadAsset<EnemyContent>("your_enemy_content");
        REPOLib.Modules.Enemies.RegisterEnemy(enemyContent);
    });
}
```

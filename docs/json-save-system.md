# JSON Save System in Unity

## Overview

JSON is one of the most popular methods for saving game data in Unity. It allows developers to serialize objects into a readable text format.

## Advantages

- Human-readable
- Easy to debug
- Supports complex data
- Cross-platform

## Limitations

- Larger file size than binary
- Not encrypted by default

## Example

```csharp
string json = JsonUtility.ToJson(playerData);
File.WriteAllText(path, json);

string loadedJson = File.ReadAllText(path);
playerData = JsonUtility.FromJson<PlayerData>(loadedJson);
```

## Best Practices

- Save files in `Application.persistentDataPath`.
- Validate data before loading.
- Create backups for important save files.

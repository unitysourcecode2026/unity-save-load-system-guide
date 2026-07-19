# Binary Save System in Unity

## Overview

A Binary Save System stores game data in a compact binary format. Compared to JSON, binary files are smaller and more difficult to edit manually.

## Advantages

- Smaller file size
- Faster read and write operations
- Better protection against casual editing
- Suitable for large save files

## Limitations

- Not human-readable
- Harder to debug
- BinaryFormatter is obsolete in modern .NET and should not be used for new projects

## Common Use Cases

- RPG save data
- Player inventory
- Game progress
- World state
- Large game saves

## Best Practices

- Use modern serialization methods instead of BinaryFormatter.
- Store save files in `Application.persistentDataPath`.
- Validate save data before loading.
- Keep backup copies of important save files.
- Include a save file version number for future compatibility.

## Security Tips

- Encrypt sensitive save data.
- Never trust modified save files.
- Validate loaded values before applying them.

## Additional Resources

Explore more Unity development tutorials and complete Unity game source code projects:

https://unitysourcecode.net

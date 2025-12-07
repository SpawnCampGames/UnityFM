# Unity AppData & Cache Locations

## User Data / AppData

| Folder | Path | Purpose |
|--------|------|---------|
| Roaming | `C:\Users\<User>\AppData\Roaming\Unity` | Unity Editor settings, Asset Store downloads, Package Manager cache |
| Local | `C:\Users\<User>\AppData\Local\Unity` | Cache, temporary files, editor logs |
| EditorPrefs | `C:\Users\<User>\AppData\Roaming\Unity\Editor-5.x` | Editor preferences and custom settings |
| Temp | `%TEMP%` → `C:\Users\<User>\AppData\Local\Temp` | Temporary build files, installers |

---

## Project-Specific Folders

| Folder | Path | Purpose |
|--------|------|---------|
| Project folder | Anywhere you created it | Contains `Assets`, `ProjectSettings`, `Packages` |
| Library | `<Project>\Library` | Auto-generated cache of imported assets |
| Temp | `<Project>\Temp` | Temporary files for building and importing |
| Logs | `<Project>\Logs` or `%LOCALAPPDATA%\Unity\Editor\Editor.log` | Editor runtime logs |

---

## Quick Notes

- Deleting the `Library` folder forces Unity to **reimport all assets**; useful for fixing broken projects.  
- `Temp` and `%TEMP%` can be safely cleared to free up space.  
- Roaming vs Local:  
  - **Roaming** travels with the user profile (settings, Asset Store cache)  
  - **Local** is machine-specific (logs, temporary data)  
- `EditorPrefs` stores your Unity editor settings per version.

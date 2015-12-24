## Incomplete Recommendations ##
(need additional thought)

| **Prefix** | **Recommended Flags** | **Description** |
|:-----------|:----------------------|:----------------|
| `info_`    | CVAR\_ROM             | Informations, like game version, build date, etc.. |
| `sys_`     | CVAR\_ROM             | Detected hardware info, like cpu, gpu, ram, etc.. |
| `dev_`     | CVAR\_DEVELOPER       | Developer settings |
| `com_`     | CVAR\_ENGINE          | Engine CVars, but not one of the following: |
| `r_`       | CVAR\_RENDERER        | Renderer settings, except image settings |
| `img_`     | CVAR\_RENDERER        | image (quality,..) settings |
| `s_`       | CVAR\_SOUND           | Audio/Sound settings |
| `in_`      | CVAR\_INPUT           | Input settings  |
| `net_`     | CVAR\_NETWORK         | Network settings |
| `ns_`      | CVAR\_NETSYNC         |  Synced over network instantly |
| `g_`       | CVAR\_GAME            | Game module CVars, except for physics |
| `phys_`    | CVAR\_GAME            | Physics settings |
| `feed_`    | CVAR\_BROWSERFEED     | Info for the serverbrowser only |
| `si_`      | CVAR\_SERVERINFO      | General server information |
| `cl_`      | CVAR\_CLIENT          | Client/User setttings |
| `fs_`      | CVAR\_ENGINE          | Filesystem settings |
| `gui_`     | ?                     | Graphical User Interface |
| `hud_`     | ?                     | Heads Up Display |
| `ai_`      | CVAR\_GAME            | Artificial Intelligence |
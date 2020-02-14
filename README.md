# Microsoft Terminal: Open In Current Directory

### Installation
- Install Microsoft Terminal from Microsoft Store.
- Create `wt.reg` file, paste code below, replace `USERNAME` with your current username, and replace `PROFILENAME` with the name of the profile you want to open.
```sh
Windows Registry Editor Version 5.00

[HKEY_CLASSES_ROOT\Directory\Background\shell\wt.PROFILENAME]
@="Open Terminal (PROFILENAME) Here"

[HKEY_CLASSES_ROOT\Directory\Background\shell\wt.PROFILENAME\command]
@="C:\\Users\\USERNAME\\AppData\\Local\\Microsoft\\WindowsApps\\wt.exe new-tab -d . -p \"PROFILENAME\""
```
- Add `wt.reg` to registry

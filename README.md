```
$ ./charge
proton installations:     4
electron installations:   7
charge:                  -3
```

This script calculates the charge of a Linux system, which is equal to the number of [Proton](https://github.com/ValveSoftware/Proton/) installations minus the number of [Electron](https://www.electronjs.org/) installations. It uses the `locate` utility to find files that are more or less unique to each package (specifically `proton_dist.tar` for Proton and either `app.asar` or `node_modules.asar` for Electron).

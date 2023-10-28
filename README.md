## filerm - PC Information Collector Tool

### Functions
- OS Information (name, kernel version, shell)
- CPU Information
- GPU Information
- Desktop Environment 
- Window Manager
- Theme (eg. Adwaita)
- Ratio of used memory to total memory
- Total Disk Size
- Memory Information (KB, MB, GB)


### Example of Usage:

```py
print("OS: " + filerm.getOS("os-name"))
print("Kernel Version: " + filerm.getOS("kernel"))
print("Default Shell: " + filerm.getOS("shell"))
print("Desktop Environment: " + filerm.getOS("desktop-env"))
print("Window Manager: " + filerm.getOS("window-mngr").capitalize())
print("Theme: " + filerm.getOS("gnome-theme"))
print("CPU: " + filerm.ReadCPU())
print("GPU: " + filerm.ReadGPU())
print("Disk Size: " + filerm.ReadDisk())
print("Memory: " + str(filerm.CurrentRam()) + " / " + filerm.ReadMemory("mb"))
print("RAM (KB): " + filerm.ReadMemory("kb"))
print("RAM (MB): " + filerm.ReadMemory("mb"))
print("RAM (GB): " + filerm.ReadMemory("gb"))
```

### Example Output:

![Filerm](./res/filerm.png)

#### Filerm licensed under the terms of MIT License.
# Nvidia Legion Image

This is a Custom Vanilla OS Image with [LenovoLegionLinux driver](https://github.com/johnfanv2/LenovoLegionLinux) included. For now it is 0.10.0, but things will change when Vanilla OS mainteiners will sync packages with debian sid. Then it will update to latest stable 0.16.0, but for now just need to wait.

> [!warning]
> I am neither the developer of Vanilla OS nor the driver. If you have any problems with the software or driver, then contact upstream.


## How to use
- Edit the /etc/abroot/abroot.json file with the `abroot config-editor edit` command.
- Change the "name" entry from something like vanilla-os/desktop to meowrosya/legion-nvidia (Note: All characters must be in lowercase).
- Now, Run `abroot upgrade -f` to switch to your custom image.

> [!important]
> My image includes _only_ the LenovoLegionLinux driver. If you need to use systemd services or GUI/CLI for tweaking the settings, you can install it manualy:
> - Type in terminal `abroot pkg add legiond python3-legion-linux`. First is systemd services and second is GUI/CLI. 
> - Then type `abroot pkg apply` and wait till completion.
> - After upgrading you must reboot system and everything _should_ work.


## Dont wanna use this image?
If you have your own image and just wanna add LenovoLegionLinux installation module to your Vib check my [modules](https://github.com/MeowRosya/vanilla-os-modules).

## Dont need Nvidia?
If you dont need image with Nvidia driver then check [Legion-Image](https://github.com/MeowRosya/Legion-Image).

# Support the drivers dev ⭐
If you found the LenovoLegionLinux driver useful than please give to the [repository](https://github.com/johnfanv2/LenovoLegionLinux).

---

# Legal Matters

Reference to any Lenovo products, services, processes, or other information and/or use of Lenovo Trademarks does not constitute or imply endorsement, sponsorship, or recommendation thereof by Lenovo.

The use of Lenovo®, Lenovo Legion™, Yoga®, IdeaPad® or other trademarks within this website and associated tools and libraries is only to provide a recognisable identifier to users to enable them to associate that these tools will work with Lenovo laptops.

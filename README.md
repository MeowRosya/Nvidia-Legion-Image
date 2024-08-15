# Nvidia Legion Image

This is a Custom Nvidia Vanilla OS Image with LenovoLegionLinux driver included. For now it is 0.10.0 version, but things will change when Vanilla OS mainteiners will sync packages with debian sid. Then it will update to latest stable 0.16.0, but for now just need to wait.

# How to use

- Edit the /etc/abroot/abroot.json file with the `abroot config-editor edit` command.
- Change the "name" entry from something like vanilla-os/desktop to meowrosya/legion-nvidia (Note: All characters must be in lowercase).
- Now, Run `abroot upgrade -f` to switch to your custom image.

## Dont need Nvidia?
If you dont need image with Nvidia driver then check [Legion-Image](https://github.com/MeowRosya/Legion-Image).


> [!caution]
> I am neither the developer of Vanilla OS nor the driver. If you have any problems with the software or driver, then contact upstream.

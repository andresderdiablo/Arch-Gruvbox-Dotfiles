Modificar línea **```GRUB_CMDLINE_LINUX_DEFAULT```** por:
```
GRUB_CMDLINE_LINUX_DEFAULT="loglevel=3 quiet splash"
```

---

Luego ejecutar en Terminal:
```
sudo grub-mkconfig -o /boot/grub/grub.cfg
```